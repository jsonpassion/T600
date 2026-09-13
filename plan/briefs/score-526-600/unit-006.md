# 2단계 — TEPS 고급 006권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-526-600/unit-006.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-526-600` (526-600, 고급) · unit 006 · 테마: 철학과 윤리 — 가치·도덕·논리
- 밴드 성격: 1+급. 신문 사설·학술 논문 수준의 고난도 문어 어휘, 미묘한 뉘앙스 형용사·동사, 고난도 콜로케이션과 관용어.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-526-600-u006
type: voca
level: 4
difficulty: advanced
tags: [teps, vocabulary, unit-006]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-526-600
score_min: 526
score_max: 600
---

# 고급 006권 — 철학과 윤리 — 가치·도덕·논리

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
1. ethics
2. morality
3. virtue
4. vice
5. utilitarianism
6. deontology
7. consequentialism
8. categorical imperative
9. egoism
10. hedonism
11. stoicism
12. nihilism
13. relativism
14. absolutism
15. determinism
16. free will
17. existentialism
18. epistemology
19. metaphysics
20. ontology
21. teleology
22. solipsism
23. empiricism
24. rationalism
25. skepticism
26. pragmatism
27. idealism
28. materialism
29. syllogism
30. tautology
31. paradox
32. dilemma
33. conundrum
34. quandary
35. deduction
36. induction
37. contradiction
38. non sequitur
39. ad hominem
40. straw man
41. slippery slope
42. red herring
43. circular reasoning
44. false dichotomy
45. sophistry
46. casuistry
47. dialectic
48. a posteriori
49. specious
50. fallacious
51. untenable
52. irrefutable
53. sound reasoning
54. veracity
55. conscience
56. integrity
57. probity
58. rectitude
59. righteousness
60. depravity
61. moral turpitude
62. moral hazard
63. moral compass
64. moral high ground
65. moral ambiguity
66. culpability
67. blameworthy
68. reprehensible
69. abhorrent
70. permissible
71. obligatory
72. prerogative
73. entitlement
74. impartiality
75. retribution
76. atonement
77. redemption
78. penance
79. remorse
80. compunction
81. scruple
82. qualm
83. expediency
84. intrinsic value
85. inalienable right
86. the greater good
87. the end justifies the means
88. the lesser of two evils
89. gray area
90. a matter of principle
91. compromise one's principles
92. practice what you preach
93. turn a blind eye
94. double standard
95. hypocrisy
96. self-righteous
97. ethos
98. precept
99. maxim
100. dogma

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-526-600/006` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
