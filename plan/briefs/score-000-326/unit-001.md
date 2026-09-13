# 2단계 — TEPS 입문 001권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-000-326/unit-001.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-000-326` (~326, 입문) · unit 001 · 테마: 일상 대화 — 인사·안부·약속의 구어 표현
- 밴드 성격: 3+급 이하. 일상·캠퍼스 대화의 구어 표현과 고등학교 수준 기본 어휘. 텝스 청해 Part 1-2와 어휘 Part 1 대화 완성에 나오는 말.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-000-326-u001
type: voca
level: 1
difficulty: beginner
tags: [teps, vocabulary, unit-001]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-000-326
score_min: 0
score_max: 326
---

# 입문 001권 — 일상 대화 — 인사·안부·약속의 구어 표현

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
1. catch up
2. make it
3. how's it going
4. long time no see
5. what's up
6. take care
7. see you around
8. keep in touch
9. drop by
10. stop by
11. come over
12. hang out
13. get together
14. run into
15. bump into
16. say hello to
17. give my regards to
18. how have you been
19. not bad
20. can't complain
21. so far so good
22. same as usual
23. nice to meet you
24. pleasure
25. introduce
26. greet
27. wave
28. shake hands
29. hug
30. promise
31. schedule
32. reschedule
33. call off
34. put off
35. postpone
36. cancel
37. confirm
38. available
39. free
40. busy
41. tied up
42. swamped
43. running late
44. on time
45. in time
46. on one's way
47. be right there
48. wait for
49. show up
50. turn up
51. stand up
52. no-show
53. sharp
54. work for
55. suit
56. convenient
57. how about
58. why don't we
59. sounds good
60. it's a deal
61. you bet
62. count me in
63. count me out
64. rain check
65. some other time
66. maybe later
67. afraid so
68. no problem
69. never mind
70. don't mention it
71. my pleasure
72. you're welcome
73. thanks anyway
74. excuse me
75. pardon
76. sorry to hear that
77. that's too bad
78. good for you
79. congratulations
80. cheer up
81. hang in there
82. take it easy
83. what a relief
84. no way
85. you're kidding
86. mean it
87. by the way
88. anyway
89. guess what
90. you know what
91. to be honest
92. have no idea
93. it depends
94. it's up to you
95. either is fine
96. look forward to
97. miss
98. remember me to
99. say goodbye
100. farewell

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-000-326/001` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
