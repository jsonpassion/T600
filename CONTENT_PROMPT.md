# 육공공 (TEPS) — 콘텐츠 생성 프롬프트

> **육공공 / Six Hundred** 앱의 단어 콘텐츠 전체를 이 리포(`~/Documents/Developer/t600-content`)에 만들어 올리는 붙여넣기용 프롬프트.
> 규격 원본은 `content.config.json` · `plan/curriculum.json` · `prompts/` · `tools/`이며, 절차 상세는 [OVERNIGHT.md](OVERNIGHT.md).
> 이 문서는 **앱 구조가 바뀐 뒤(2026-09-14) 기준**으로 콘텐츠가 앱에 맞게 들어가도록 필요한 사실을 한곳에 모았다.

## 사용법

1. 터미널에서 `cd ~/Documents/Developer/t600-content && claude` 로 이 리포를 연다.
2. 아래 **붙여넣기 프롬프트** 블록 전체를 그대로 붙여넣는다. 첫 단어 `ultracode`가 멀티 에이전트 병렬 실행을 켠다.
3. 중간에 끊겨도 같은 프롬프트를 다시 붙여넣으면 된다. 이미 쓰인 권은 동결되고 `todo`에 남은 권만 이어서 쓴다.

## 앱이 이 콘텐츠를 읽는 방식

| 항목 | 내용 |
|---|---|
| 앱 | 육공공 / Six Hundred (TEPS, 타깃 `T600`) — 한국인 텝스 수험생, 한국어 UI |
| 레벨 방식 | **점수대 모드**(4밴드, 사용자가 고름): `score-000-326`(~326) · `score-327-452` · `score-453-525` · `score-526-600` |
| 권 구성 | 밴드마다 **10권 × 100단어 = 40권 4,000단어**, 10단어 = 1챕터, 책장은 번호 권(`volumes`) |
| 무료 | 밴드마다 1권(10챕터) |
| 줄 형식 | `- word \| 한국어 뜻 \| /IPA/ \| TIP \| English example \| 예문 번역` |
| 카드 | 앞면 = 표제어 + IPA, 뒷면 = 뜻·TIP·예문·번역, TTS = 영어 단어/예문 + 한국어 뜻 |
| 중복 | 트랙 전체(4밴드 통틀어) 표제어 중복 금지, 대소문자 무시 |
| 배포 | `manifest.json` → `https://raw.githubusercontent.com/jsonpassion/T600/main/manifest.json` |

## 붙여넣기 프롬프트

```
ultracode. 이 리포(현재 디렉토리)는 육공공 / Six Hundred 앱의 단어 콘텐츠 리포다. main 에 push 하면 앱에 배포된다.
아래 사실과 품질 기준을 지키며 OVERNIGHT.md 절차로 전체 단어책을 끝까지 만들고 배포하라.

[앱 구조]
- 앱 : 육공공 / Six Hundred (TEPS, 타깃 T600) — 한국인 텝스 수험생, 한국어 UI
- 레벨 방식 : 점수대 모드(4밴드, 사용자가 고름): score-000-326(~326) · score-327-452 · score-453-525 · score-526-600
- 권 구성 : 밴드마다 10권 × 100단어 = 40권 4,000단어, 10단어 = 1챕터, 책장은 번호 권(volumes)
- 무료 : 밴드마다 1권(10챕터)
- 줄 형식 : - word | 한국어 뜻 | /IPA/ | TIP | English example | 예문 번역
- 카드 : 앞면 = 표제어 + IPA, 뒷면 = 뜻·TIP·예문·번역, TTS = 영어 단어/예문 + 한국어 뜻
- 중복 : 트랙 전체(4밴드 통틀어) 표제어 중복 금지, 대소문자 무시
- 배포 : manifest.json → https://raw.githubusercontent.com/jsonpassion/T600/main/manifest.json

[품질 기준]
- 텝스 어휘 파트 구성을 반영: Part 1 구어 대화 완성(구동사·회화 관용 표현)과 Part 2 문어 문장 완성(콜로케이션·격식 동사·형용사). 청해·독해 빈출 어휘도 포함.
- 밴드 난이도 경계를 지킨다: ~326은 고교~일상 구어, 327-452는 사회·비즈니스 빈출·기본 구동사, 453-525는 시사·학술 문어, 526-600은 사설·논문급 고난도·뉘앙스 어휘.
- 표제어는 단어뿐 아니라 구동사·콜로케이션·관용구 허용(텝스 특성). 토익 비즈니스 어휘로 채우지 않는다.
- IPA는 미국식, 구 전체를 표기. 뜻은 시험에서 묻는 뜻 먼저 최대 2개.
- TIP(한국어 45자 이내)은 혼동어 구별·짝 전치사·뉘앙스 차이·빈출 콜로케이션 중 가장 효과적인 한 줄. 뜻 반복 금지.
- 예문 8–16단어: 구어 표현은 대화 한 줄, 문어 어휘는 신문·학술 톤.

[절차]
1) python3 tools/plan.py clear-dummy && python3 tools/plan.py wordlist-briefs
2) 밴드마다 에이전트 1개씩 병렬: plan/briefs/wordlist-<band>.md 를 읽고 그대로 수행해 plan/wordlists/<band>.md 작성.
3) python3 tools/plan.py merge — SHORT 가 나오면 그 권의 후보만 보충하는 에이전트를 돌리고 merge 를 반복해 0 short 로 만든다.
4) python3 tools/plan.py briefs
5) plan/briefs/<band>/unit-NNN.md 하나당 에이전트 1개, 동시 최대 12개. 각 에이전트는 brief 를 그대로 수행해 자기 파일 하나만 쓰고
   python3 tools/validate_content.py --unit <band>/NNN 이 0 errors 가 될 때까지 자기 파일의 오류 줄만 고친다.
6) python3 tools/validate_content.py 전체 0 errors 가 될 때까지 python3 tools/plan.py todo 의 목록만 5)를 반복.
7) 밴드 하나가 끝날 때마다 python3 tools/build_manifest.py → git add content plan manifest.json → 커밋 → push (중간 배포 허용).

[금지]
- 표제어 선정과 배정은 반드시 `plan.py merge` 결과만 따른다. 작성 에이전트는 단어를 고르거나 바꾸지 않는다.
- 실제 기출문제·유료 교재 문장을 옮기지 않는다. 예문·TIP은 전부 새로 쓴다.
- `docs/`, `privacy.md`, `terms.md`, `README.md`는 건드리지 않는다(사이트·약관은 별도 관리).
- `tools/*.py`에 버그가 보이면 고치지 말고 멈춰서 보고한다(모든 앱 리포가 같은 도구를 공유함).
- 출시 전이므로 더미 권 삭제는 괜찮다. **출시 후에는 표제어 철자 변경·삭제 금지** — 카드 ID(`<unit id>-<표제어>`)에 학습 기록이 묶여 있다.

[완료 조건]
- python3 tools/validate_content.py 0 errors, 경고는 권당 3개 이하.
- python3 tools/plan.py todo 가 "nothing to do", status 의 written 합계 = 40권, 총 4,000단어, dummy 권 0개.
- python3 tools/build_manifest.py --check 가 up to date, push 후 raw manifest 의 version 이 로컬과 같다.
끝나면 급수(밴드)별 권 수·단어 수, 경고 수, 커밋 해시, raw manifest 버전을 보고하라.
```

## 완료 확인 (사람이 직접)

```bash
python3 tools/plan.py status
python3 tools/validate_content.py --quiet | tail -1
python3 tools/build_manifest.py --check
curl -s https://raw.githubusercontent.com/jsonpassion/T600/main/manifest.json | head -3
```
