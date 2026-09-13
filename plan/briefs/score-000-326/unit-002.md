# 2단계 — TEPS 입문 002권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-000-326/unit-002.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-000-326` (~326, 입문) · unit 002 · 테마: 캠퍼스 생활 — 수강신청·과제·동아리
- 밴드 성격: 3+급 이하. 일상·캠퍼스 대화의 구어 표현과 고등학교 수준 기본 어휘. 텝스 청해 Part 1-2와 어휘 Part 1 대화 완성에 나오는 말.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-000-326-u002
type: voca
level: 1
difficulty: beginner
tags: [teps, vocabulary, unit-002]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-000-326
score_min: 0
score_max: 326
---

# 입문 002권 — 캠퍼스 생활 — 수강신청·과제·동아리

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
1. sign up for
2. register
3. enroll
4. course
5. lecture
6. professor
7. instructor
8. teaching assistant
9. major in
10. minor
11. credit
12. semester
13. freshman
14. sophomore
15. junior
16. senior
17. graduate
18. degree
19. transcript
20. grade
21. grade point average
22. pass
23. fail
24. drop a class
25. prerequisite
26. required course
27. elective
28. syllabus
29. attendance
30. absent
31. skip class
32. be late for
33. assignment
34. homework
35. due
36. deadline
37. hand in
38. turn in
39. submit
40. extension
41. essay
42. report
43. paper
44. research
45. presentation
46. group project
47. team up with
48. figure out
49. work on
50. look up
51. go over
52. review
53. brush up on
54. cram
55. study for
56. midterm
57. final exam
58. quiz
59. score
60. pop quiz
61. open-book
62. cheat on
63. take notes
64. textbook
65. handout
66. library
67. overdue
68. dormitory
69. roommate
70. campus
71. cafeteria
72. student ID
73. tuition
74. scholarship
75. apply for
76. application
77. club
78. join
79. member
80. activity
81. volunteer
82. orientation
83. advisor
84. office hours
85. be good at
86. struggle with
87. fall behind
88. keep up with
89. catch on
90. get the hang of
91. make progress
92. improve
93. effort
94. focus on
95. concentrate
96. stay up late
97. pull an all-nighter
98. give up
99. try one's best
100. do well on

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-000-326/002` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
