# Six Hundred Content — TEPS 어휘 콘텐츠 리포

> **Six Hundred(육공공)** — 만점 600에서 따온 이름.
> [NINE90](https://github.com/jsonpassion/NINE90)(TOEIC 트랙)과 동일한 콘텐츠 파이프라인을 쓰는
> TEPS 트랙 리포지토리 — 앱은 manifest URL 하나로 이 리포의 콘텐츠를 통째로 동기화합니다.

**현재 상태: 규격·도구·생성 파이프라인만 존재.** 단어는 [OVERNIGHT.md](OVERNIGHT.md) 절차로 밤새 병렬 생성한다.

## 구조

```
content.config.json               ← 트랙 규격: 밴드·권 수·언어·표기 (도구가 모두 이것을 읽는다)
plan/curriculum.json              ← 밴드별 10권 테마
prompts/wordlist.md               ← 1단계: 밴드별 후보 표제어 프롬프트
prompts/unit.md                   ← 2단계: 배정된 100단어로 권 파일 쓰기 프롬프트
tools/plan.py                     ← 후보 병합·전역 중복 제거·100개 배정·brief 생성·todo
tools/validate_content.py         ← 형식·표기·중복·배정 일치 검증 (0 errors 필수)
tools/build_manifest.py           ← manifest.json 생성
content/voca/{band}/unit-NNN.md   ← 1파일 = 1권 = 100단어 (10단어 = 1챕터)
OVERNIGHT.md                      ← 밤샘 병렬 생성 런북 + 붙여넣기용 오케스트레이션 프롬프트
```

## 점수 밴드 (New TEPS 0–600, 공인 등급 기준)

| band_id | 레벨 | 라벨 | 성격 |
|---|---|---|---|
| `score-000-326` | 1 · beginner | ~326 (3+급 이하) | 기초 어휘 · 구어 표현 |
| `score-327-452` | 2 · intermediate | 327–452 (2급·2+급, 국가공인) | 빈출 어휘 · 콜로케이션 |
| `score-453-525` | 3 · upper-intermediate | 453–525 (1급) | 문어체 고급 어휘 · 구동사 |
| `score-526-600` | 4 · advanced | 526–600 (1+급) | 최고난도 어휘 · 관용어 · 시사 |

## NINE90 형식과 동일 — 권 번호 책장

TOEIC 트랙과 같은 **권 번호("N권") 책장**을 씁니다. `unit_title` 계열 frontmatter는 필요 없습니다
(있어도 무시). 텝스 어휘 영역의 여섯 갈래(구어 표현·문어 어휘·콜로케이션·구동사·관용어·시사/학술)를
매 권 100단어 안에 고르게 섞고, 레벨이 올라갈수록 문어체 고급 어휘 비중을 높입니다.

그 외 단어 줄 형식은 NINE90 v2와 동일합니다:

```
- word | 한국어 뜻 | /IPA/ | 암기 힌트 | English example | 예문 번역
```

샘플: [content/voca/score-526-600/unit-001.md](content/voca/score-526-600/unit-001.md)
(형식 시연용 10단어 — 실제 유닛은 100단어).

## 콘텐츠 규칙

- 유닛당 **정확히 100단어**, 10단어 = 1챕터 (앱의 회독 단위)
- **밴드 내 중복 = 오류**, 밴드 간 중복 = 경고(허용 — 레벨이 올라가면 재등장 가능)
- 필드 안에 파이프(`|`) 금지 (구분자 전용)
- 카드 ID = `{파일 id}-{표제어 slug}` — 줄 순서와 무관하지만, **출시 후 표제어 철자 변경·삭제는 금지**
  (사용자 학습 진도가 카드 ID에 매여 있음). 추가는 새 유닛 파일로.
- `manifest.json`의 `profile.free_chapters`(기본 10 = 1권) = 밴드마다 무료로 열리는 챕터 수
  (앱이 원격 설정으로 읽음)

## 워크플로

단어 생성은 [OVERNIGHT.md](OVERNIGHT.md) 한 곳에 정리돼 있다 (후보 목록 → 전역 중복 제거·배정 → 권별 병렬 작성 → 검증).

```bash
python3 tools/plan.py status         # 진행 상황
python3 tools/validate_content.py    # 0 errors 필수
python3 tools/build_manifest.py
git add content plan manifest.json && git commit && git push
```

앱은 raw.githubusercontent.com의 manifest.json 버전 변경을 감지해 바뀐 파일만 내려받습니다
(sha256 검증 포함). raw CDN 캐시 특성상 push 후 매니페스트 반영까지 ~5분 걸릴 수 있습니다.

## 상표 고지

TEPS는 서울대학교 TEPS관리위원회의 등록 상표입니다. 이 리포지토리와 관련 앱은
서울대학교 TEPS관리위원회와 무관하며, 서울대학교 TEPS관리위원회의 제휴·보증·승인을 받지 않았습니다. 모든 콘텐츠는 자체 제작이며
실제 기출문제를 포함하지 않습니다.

© 2026 ForgeLab
