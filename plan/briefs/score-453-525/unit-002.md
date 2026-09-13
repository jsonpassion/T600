# 2단계 — TEPS 중상급 002권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-453-525/unit-002.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-453-525` (453-525, 중상급) · unit 002 · 테마: 경제 심화 — 경기·투자·무역
- 밴드 성격: 1급. 시사·학술 지문의 문어체 어휘, 격식 표현, 관용어와 다의 구동사. 어휘 Part 2 문장 완성 20문항의 주력 구간.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-453-525-u002
type: voca
level: 3
difficulty: upper-intermediate
tags: [teps, vocabulary, unit-002]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-453-525
score_min: 453
score_max: 525
---

# 중상급 002권 — 경제 심화 — 경기·투자·무역

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
1. depression
2. downturn
3. slump
4. stagnation
5. stagflation
6. rebound
7. bubble
8. stimulus
9. austerity
10. public debt
11. bankruptcy
12. insolvent
13. liquidity
14. creditor
15. debtor
16. liability
17. equity
18. portfolio
19. diversify
20. securities
21. shareholder
22. venture capital
23. return on investment
24. yield
25. speculate
26. volatility
27. bull market
28. bear market
29. plunge
30. surge
31. curb
32. quota
33. protectionism
34. free trade agreement
35. trade barrier
36. dumping
37. customs duty
38. supply chain
39. outsource
40. globalization
41. emerging market
42. productivity
43. labor market
44. monopoly
45. antitrust
46. merger
47. acquisition
48. takeover
49. conglomerate
50. subsidiary
51. profit margin
52. overhead
53. go under
54. cash in on
55. write off
56. prop up
57. bottom out
58. level off
59. devalue
60. capital flight
61. foreign direct investment
62. inflow
63. sluggish
64. robust
65. buoyant
66. lucrative
67. incentive
68. tax break
69. levy
70. indicator
71. quarterly
72. soft landing
73. initial public offering
74. valuation
75. scarcity
76. deregulation
77. privatize
78. state-owned
79. trade war
80. disparity
81. contraction
82. upturn
83. overheat
84. glut
85. shortfall
86. oversupply
87. nosedive
88. tumble
89. rally
90. windfall
91. stake
92. hedge
93. bond yield
94. brokerage
95. capital gains
96. credit rating
97. creditworthy
98. divest
99. downgrade
100. hostile takeover

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-453-525/002` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
