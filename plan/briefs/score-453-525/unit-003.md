# 2단계 — TEPS 중상급 003권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-453-525/unit-003.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-453-525` (453-525, 중상급) · unit 003 · 테마: 과학 기술 — 연구·실험·혁신
- 밴드 성격: 1급. 시사·학술 지문의 문어체 어휘, 격식 표현, 관용어와 다의 구동사. 어휘 Part 2 문장 완성 20문항의 주력 구간.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-453-525-u003
type: voca
level: 3
difficulty: upper-intermediate
tags: [teps, vocabulary, unit-003]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-453-525
score_min: 453
score_max: 525
---

# 중상급 003권 — 과학 기술 — 연구·실험·혁신

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
1. control group
2. replicate
3. validate
4. falsify
5. anomaly
6. phenomenon
7. specimen
8. sample size
9. methodology
10. parameter
11. calibrate
12. quantify
13. correlation
14. causation
15. statistically significant
16. margin of error
17. innovate
18. commercialize
19. automation
20. robotics
21. nanotechnology
22. biotechnology
23. genetic engineering
24. genome
25. clone
26. synthesize
27. synthetic
28. compound
29. molecule
30. particle
31. nuclear fission
32. fusion
33. radiation
34. conductor
35. circuit
36. semiconductor
37. orbit
38. satellite
39. spacecraft
40. velocity
41. momentum
42. thermal
43. combustion
44. catalyst
45. dissolve
46. evaporate
47. condense
48. compress
49. dilute
50. apparatus
51. augmented reality
52. simulation
53. extrapolate
54. infer
55. deduce
56. theorem
57. formula
58. equation
59. derive
60. exponential
61. trajectory
62. precision
63. rigorous
64. systematic
65. trial and error
66. break new ground
67. pioneer
68. stumble upon
69. disprove
70. debunk
71. groundbreaking
72. revolutionize
73. disruptive
74. iteration
75. embed
76. transmit
77. frequency
78. wavelength
79. spectrum
80. quantum
81. organism
82. microorganism
83. mutation
84. peer-reviewed
85. dependent variable
86. controlled experiment
87. meticulous
88. proof of concept
89. research and development
90. feasibility
91. push the envelope
92. at the forefront of
93. cast doubt on
94. hit upon
95. come up against
96. magnify
97. refraction
98. inertia
99. kinetic energy
100. electromagnetic

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-453-525/003` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
