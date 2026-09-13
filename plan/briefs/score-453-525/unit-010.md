# 2단계 — TEPS 중상급 010권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-453-525/unit-010.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-453-525` (453-525, 중상급) · unit 010 · 테마: 구동사 집중 — 문맥마다 뜻이 바뀌는 구동사
- 밴드 성격: 1급. 시사·학술 지문의 문어체 어휘, 격식 표현, 관용어와 다의 구동사. 어휘 Part 2 문장 완성 20문항의 주력 구간.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-453-525-u010
type: voca
level: 3
difficulty: upper-intermediate
tags: [teps, vocabulary, unit-010]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-453-525
score_min: 453
score_max: 525
---

# 중상급 010권 — 구동사 집중 — 문맥마다 뜻이 바뀌는 구동사

- word | 한국어 뜻 | /IPA/ | TIP | English example | 예문 번역
```
단어 줄은 배정 순서대로 **정확히 100줄**, 필드 6개, 구분자는 ` | `. 어떤 필드에도 `|`를 추가로 쓰지 않는다.

## 필드별 기준 — 카드 앞면은 word·IPA, 뒷면은 뜻·TIP·예문·번역
1. **word**: 배정표 그대로.
2. **한국어 뜻**: 텝스에서 묻는 뜻을 먼저, 최대 두 개를 쉼표로. 품사가 헷갈리면 괄호. 예: `이의를 제기하다`, `(가격이) 터무니없는`.
3. **IPA**: 미국식, `/ /` 안에. 구·관용어도 전체를 적는다. 예: `/teɪk ˈɪʃuː wɪð/`.
4. **TIP** (뒷면 노란 TIP 칸, 한국어 45자 이내): 이 단어를 **시험장에서 맞히게 하는 한 줄**. 아래 중 가장 효과적인 하나를 고른다.
   - 어원 분해: `ex(밖으로)+orbit(궤도) → 궤도를 벗어난 값`
   - 콜로케이션·짝: `take issue ‘with’ 전치사까지 한 덩어리`
   - 혼동어 구분: `adopt=채택, adapt=적응 — o는 option`
   - 뉘앙스·격식: `구어 hang in there, 문어 persevere`
   - 텝스 출제 포인트: `대화 완성 빈출 — 거절할 때 쓰는 완곡 표현`
   뜻을 다시 쓰거나 "중요한 단어"처럼 정보 없는 말은 금지.
5. **English example**: 텝스 톤의 자연스러운 한 문장, 8–16단어. 구어 표현은 대화 한 줄(따옴표 없이), 문어 어휘는 신문·학술 문장.
   표제어가 문장에 그대로(시제·수 변화 허용) 들어가야 한다. 너무 쉬운 교과서 문장(`This is a book.` 류) 금지.
6. **예문 번역**: 직역투 없이 자연스러운 한국어 한 문장.

## 배정된 표제어 (이 순서대로 100줄)
1. bring about
2. come about
3. account for
4. make up
5. make out
6. put up with
7. set out
8. turn out
9. turn over
10. take over
11. take on
12. take in
13. take after
14. give out
15. give up on
16. hold back
17. hold off
18. hold out
19. come up with
20. come across
21. come down to
22. come through
23. come off
24. go through
25. go off
26. go along with
27. go without
28. fall through
29. fall back on
30. fall out
31. get around
32. get at
33. run out of
34. run over
35. run down
36. pick up
37. break out
38. break off
39. break into
40. break up
41. draw on
42. wear out
43. wind up
44. lay out
45. pass up
46. pass out
47. pass on
48. rule out
49. single out
50. stand for
51. stand up for
52. call for
53. call on
54. keep up
55. live up to
56. cut in
57. do away with
58. bring down
59. bring on
60. boil down to
61. butt in
62. cave in
63. clamp down on
64. crack down on
65. hand over
66. jot down
67. kick off
68. pan out
69. see through
70. pull off
71. act up
72. back out
73. bear on
74. bear with
75. blow over
76. bring round
77. carry off
78. carry over
79. come by
80. come into
81. cut out
82. eat into
83. edge out
84. factor in
85. fill in
86. get through
87. give way
88. go back on
89. hang on
90. kick in
91. knock off
92. let up
93. live down
94. make for
95. miss out on
96. own up to
97. play down
98. play up
99. put across
100. put out

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-453-525/010` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
