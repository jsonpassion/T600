# 2단계 — TEPS 입문 006권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-000-326/unit-006.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-000-326` (~326, 입문) · unit 006 · 테마: 직장 첫걸음 — 출근·회의·보고
- 밴드 성격: 3+급 이하. 일상·캠퍼스 대화의 구어 표현과 고등학교 수준 기본 어휘. 텝스 청해 Part 1-2와 어휘 Part 1 대화 완성에 나오는 말.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-000-326-u006
type: voca
level: 1
difficulty: beginner
tags: [teps, vocabulary, unit-006]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-000-326
score_min: 0
score_max: 326
---

# 입문 006권 — 직장 첫걸음 — 출근·회의·보고

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
1. commute
2. clock in
3. clock out
4. punch in
5. call in sick
6. day off
7. take a day off
8. work overtime
9. shift
10. night shift
11. colleague
12. coworker
13. boss
14. manager
15. supervisor
16. employee
17. employer
18. intern
19. internship
20. staff
21. department
22. team leader
23. new hire
24. hire
25. fire
26. quit
27. resign
28. retire
29. promotion
30. get promoted
31. pay raise
32. salary
33. wage
34. paycheck
35. bonus
36. meeting
37. set up a meeting
38. call a meeting
39. agenda
40. attend
41. conference room
42. minutes
43. give a presentation
44. meet the deadline
45. behind schedule
46. on schedule
47. ahead of schedule
48. task
49. workload
50. in charge of
51. be responsible for
52. duty
53. project
54. fill in for
55. cover for
56. learn the ropes
57. get used to
58. training
59. trainee
60. résumé
61. job interview
62. application form
63. qualification
64. experience
65. position
66. full-time
67. part-time
68. office
69. desk
70. copy machine
71. printer
72. email
73. reply
74. forward
75. attach
76. file
77. document
78. check in with
79. follow up
80. get back to
81. touch base
82. brainstorm
83. idea
84. propose
85. agree
86. disagree
87. opinion
88. decide
89. discuss
90. look over
91. approve
92. work from home
93. lunch break
94. take a break
95. business trip
96. client
97. company
98. hardworking
99. teamwork
100. cooperate

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-000-326/006` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
