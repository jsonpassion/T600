# 2단계 — TEPS 입문 005권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-000-326/unit-005.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-000-326` (~326, 입문) · unit 005 · 테마: 건강과 병원 — 증상·진료·약
- 밴드 성격: 3+급 이하. 일상·캠퍼스 대화의 구어 표현과 고등학교 수준 기본 어휘. 텝스 청해 Part 1-2와 어휘 Part 1 대화 완성에 나오는 말.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-000-326-u005
type: voca
level: 1
difficulty: beginner
tags: [teps, vocabulary, unit-005]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-000-326
score_min: 0
score_max: 326
---

# 입문 005권 — 건강과 병원 — 증상·진료·약

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
1. sick
2. ill
3. illness
4. disease
5. health
6. healthy
7. hurt
8. pain
9. painful
10. ache
11. headache
12. stomachache
13. toothache
14. backache
15. fever
16. catch a cold
17. flu
18. cough
19. sneeze
20. runny nose
21. sore throat
22. stuffy nose
23. symptom
24. dizzy
25. tired
26. exhausted
27. feel sick
28. throw up
29. vomit
30. diarrhea
31. allergic to
32. rash
33. itchy
34. swollen
35. bleed
36. blood
37. wound
38. injury
39. injure
40. bruise
41. scratch
42. burn
43. sprain
44. broken bone
45. cast
46. bandage
47. hospital
48. clinic
49. doctor
50. nurse
51. patient
52. see a doctor
53. checkup
54. examine
55. test results
56. x-ray
57. blood pressure
58. temperature
59. take one's temperature
60. diagnose
61. treat
62. cure
63. heal
64. recover
65. get better
66. get well soon
67. feel better
68. come down with
69. under the weather
70. medicine
71. pill
72. tablet
73. drug
74. pharmacy
75. prescription
76. prescribe
77. take medicine
78. side effect
79. dose
80. painkiller
81. vitamin
82. emergency
83. ambulance
84. emergency room
85. surgery
86. operation
87. insurance
88. fill out
89. form
90. waiting room
91. be in the hospital
92. stay in bed
93. get some rest
94. sleep
95. lack of sleep
96. stress
97. stressed out
98. exercise
99. diet
100. lose weight

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-000-326/005` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
