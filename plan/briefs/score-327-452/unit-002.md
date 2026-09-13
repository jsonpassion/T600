# 2단계 — TEPS 중급 002권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-327-452/unit-002.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-327-452` (327-452, 중급) · unit 002 · 테마: 돈과 경제 기초 — 예산·대출·물가
- 밴드 성격: 2급·2+급(국가공인 진입). 비즈니스·사회 전반의 빈출 어휘, 기본 콜로케이션과 구동사. 서울대 대학원 최소 기준 327점을 넘기는 구간.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-327-452-u002
type: voca
level: 2
difficulty: intermediate
tags: [teps, vocabulary, unit-002]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-327-452
score_min: 327
score_max: 452
---

# 중급 002권 — 돈과 경제 기초 — 예산·대출·물가

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
1. surplus
2. deficit
3. expense
4. expenditure
5. cut back on
6. set aside
7. make ends meet
8. live within one's means
9. tighten one's belt
10. take out a loan
11. pay off
12. pay back
13. lender
14. interest rate
15. mortgage
16. down payment
17. credit score
18. debt
19. owe
20. repay
21. default
22. go bankrupt
23. go broke
24. collateral
25. inflation
26. deflation
27. price hike
28. soar
29. skyrocket
30. plummet
31. fluctuate
32. stabilize
33. cost of living
34. consumer price index
35. purchasing power
36. recession
37. economic downturn
38. boom
39. recovery
40. gross domestic product
41. disposable income
42. tax deduction
43. tax return
44. revenue
45. break even
46. turn a profit
47. in the red
48. in the black
49. bottom line
50. raise funds
51. invest
52. investor
53. dividend
54. stock market
55. currency
56. exchange rate
57. depreciate
58. appreciate
59. withdraw
60. deposit
61. savings account
62. balance
63. overdraft
64. transaction
65. wire transfer
66. foot the bill
67. chip in
68. reimburse
69. allowance
70. subsidy
71. supply and demand
72. shortage
73. scarce
74. commodity
75. cost-effective
76. economical
77. economic
78. frugal
79. thrifty
80. extravagant
81. splurge
82. be worth it
83. estimate
84. financial crisis
85. bailout
86. stimulus package
87. interest-free
88. monetary
89. fiscal
90. fiscal year
91. asset
92. net worth
93. affluent
94. well-off
95. strapped for cash
96. cash flow
97. consumer spending
98. household debt
99. tariff
100. trade deficit

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-327-452/002` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
