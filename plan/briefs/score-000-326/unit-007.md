# 2단계 — TEPS 입문 007권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-000-326/unit-007.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-000-326` (~326, 입문) · unit 007 · 테마: 집과 생활 — 이사·수리·이웃
- 밴드 성격: 3+급 이하. 일상·캠퍼스 대화의 구어 표현과 고등학교 수준 기본 어휘. 텝스 청해 Part 1-2와 어휘 Part 1 대화 완성에 나오는 말.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-000-326-u007
type: voca
level: 1
difficulty: beginner
tags: [teps, vocabulary, unit-007]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-000-326
score_min: 0
score_max: 326
---

# 입문 007권 — 집과 생활 — 이사·수리·이웃

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
1. move
2. move in
3. move out
4. moving company
5. apartment
6. landlord
7. tenant
8. rent
9. security deposit
10. lease
11. utility bill
12. electricity
13. neighbor
14. next door
15. upstairs
16. downstairs
17. noise
18. noisy
19. quiet
20. repair
21. fix
22. break down
23. broken
24. leak
25. faucet
26. pipe
27. plumber
28. electrician
29. handyman
30. toolbox
31. hammer
32. nail
33. screw
34. ladder
35. light bulb
36. out of order
37. clogged
38. drain
39. sink
40. toilet
41. bathroom
42. bedroom
43. living room
44. kitchen
45. furniture
46. couch
47. closet
48. drawer
49. shelf
50. carpet
51. floor
52. ceiling
53. wall
54. window
55. curtain
56. roof
57. garage
58. yard
59. garden
60. lawn
61. mow the lawn
62. water the plants
63. do the dishes
64. do the laundry
65. vacuum
66. sweep
67. mop
68. dust
69. tidy up
70. clean up
71. take out the trash
72. garbage
73. messy
74. throw away
75. get rid of
76. set up
77. put together
78. hang up
79. plug in
80. turn on
81. turn off
82. heater
83. air conditioner
84. washing machine
85. lock
86. key
87. doorbell
88. knock
89. neighborhood
90. settle in
91. feel at home
92. make yourself at home
93. housewarming party
94. spacious
95. cozy
96. crowded
97. comfortable
98. housemate
99. pet
100. feed

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-000-326/007` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
