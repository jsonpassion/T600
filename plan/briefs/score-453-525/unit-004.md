# 2단계 — TEPS 중상급 004권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-453-525/unit-004.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-453-525` (453-525, 중상급) · unit 004 · 테마: 의학과 보건 — 질병·치료·임상
- 밴드 성격: 1급. 시사·학술 지문의 문어체 어휘, 격식 표현, 관용어와 다의 구동사. 어휘 Part 2 문장 완성 20문항의 주력 구간.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-453-525-u004
type: voca
level: 3
difficulty: upper-intermediate
tags: [teps, vocabulary, unit-004]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-453-525
score_min: 453
score_max: 525
---

# 중상급 004권 — 의학과 보건 — 질병·치료·임상

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
1. prognosis
2. chronic
3. acute
4. contagious
5. infectious
6. epidemic
7. pandemic
8. outbreak
9. pathogen
10. bacterial
11. immune system
12. immunity
13. herd immunity
14. vaccinate
15. antibody
16. antibiotic
17. drug-resistant
18. dosage
19. over-the-counter
20. adverse reaction
21. inflammation
22. nausea
23. dizziness
24. fatigue
25. insomnia
26. obesity
27. diabetes
28. hypertension
29. cardiovascular
30. stroke
31. tumor
32. malignant
33. benign
34. chemotherapy
35. surgical
36. anesthesia
37. transplant
38. donor
39. recuperate
40. relapse
41. remission
42. terminal illness
43. palliative care
44. hospice
45. clinical trial
46. placebo
47. efficacy
48. double-blind
49. cohort
50. informed consent
51. pharmaceutical
52. generic drug
53. medication
54. remedy
55. alleviate
56. relieve
57. soothe
58. aggravate
59. exacerbate
60. deteriorate
61. afflict
62. suffer from
63. pass away
64. fight off
65. pull through
66. on the mend
67. wear off
68. airborne
69. quarantine
70. sanitation
71. hygiene
72. sterile
73. disinfect
74. epidemiology
75. mortality rate
76. public health
77. malnutrition
78. deficiency
79. nutrient
80. metabolism
81. hormone
82. genetic predisposition
83. hereditary
84. congenital
85. disorder
86. syndrome
87. dementia
88. therapeutic
89. physician
90. pediatrician
91. surgeon
92. practitioner
93. referral
94. screening
95. vital signs
96. respiratory
97. fracture
98. hemorrhage
99. coma
100. paralysis

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-453-525/004` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
