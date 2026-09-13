# 2단계 — TEPS 중급 009권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-327-452/unit-009.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-327-452` (327-452, 중급) · unit 009 · 테마: 광고와 마케팅 — 홍보·브랜드·소비자
- 밴드 성격: 2급·2+급(국가공인 진입). 비즈니스·사회 전반의 빈출 어휘, 기본 콜로케이션과 구동사. 서울대 대학원 최소 기준 327점을 넘기는 구간.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-327-452-u009
type: voca
level: 2
difficulty: intermediate
tags: [teps, vocabulary, unit-009]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-327-452
score_min: 327
score_max: 452
---

# 중급 009권 — 광고와 마케팅 — 홍보·브랜드·소비자

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
1. advertise
2. commercial
3. campaign
4. promote
5. publicity
6. public relations
7. press release
8. brand image
9. brand awareness
10. logo
11. slogan
12. tagline
13. jingle
14. mascot
15. target audience
16. market research
17. focus group
18. consumer
19. customer base
20. clientele
21. potential customer
22. word of mouth
23. influencer
24. endorse
25. sponsor
26. testimonial
27. customer review
28. billboard
29. flyer
30. brochure
31. banner
32. prime time
33. airtime
34. infomercial
35. launch
36. roll out
37. unveil
38. hit the shelves
39. markdown
40. clearance sale
41. special offer
42. limited-time offer
43. buy one get one free
44. voucher
45. rewards program
46. free sample
47. giveaway
48. competitive edge
49. competitor
50. market share
51. niche
52. differentiate
53. stand out
54. appeal to
55. catch someone's eye
56. eye-catching
57. persuasive
58. misleading
59. false advertising
60. exaggerate
61. hype
62. gimmick
63. packaging
64. label
65. window display
66. retailer
67. wholesale
68. distributor
69. merchandise
70. outlet
71. franchise
72. chain store
73. impulse buy
74. shop around
75. splurge on
76. window-shopping
77. trend
78. fad
79. craze
80. all the rage
81. go out of style
82. reputation
83. credibility
84. fan base
85. repeat customer
86. customer satisfaction
87. ad agency
88. pitch
89. print media
90. trade show
91. booth
92. showcase
93. demonstration
94. hard sell
95. price tag
96. high-end
97. luxury
98. premium
99. store brand
100. knockoff

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-327-452/009` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
