# 2단계 — TEPS 고급 007권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-526-600/unit-007.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-526-600` (526-600, 고급) · unit 007 · 테마: 법률과 규제 심화 — 소송·판결·입법
- 밴드 성격: 1+급. 신문 사설·학술 논문 수준의 고난도 문어 어휘, 미묘한 뉘앙스 형용사·동사, 고난도 콜로케이션과 관용어.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-526-600-u007
type: voca
level: 4
difficulty: advanced
tags: [teps, vocabulary, unit-007]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-526-600
score_min: 526
score_max: 600
---

# 고급 007권 — 법률과 규제 심화 — 소송·판결·입법

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
1. litigation
2. litigant
3. adjudicate
4. arbitration
5. injunction
6. subpoena
7. affidavit
8. deposition
9. indict
10. arraignment
11. acquittal
12. overturn a conviction
13. uphold a ruling
14. appellate court
15. jurisprudence
16. precedent
17. set a precedent
18. landmark ruling
19. statute of limitations
20. ordinance
21. decree
22. codify
23. legislate
24. annul
25. nullify
26. abrogate
27. omnibus bill
28. sunset clause
29. bicameral
30. come into force
31. tribunal
32. magistrate
33. counsel
34. prosecute
35. testimony
36. perjury
37. cross-examination
38. admissible
39. hearsay
40. burden of proof
41. beyond a reasonable doubt
42. presumption of innocence
43. habeas corpus
44. plea bargain
45. extradition
46. tort
47. punitive damages
48. class action
49. file suit
50. bring charges against
51. mistrial
52. hung jury
53. hand down a sentence
54. commute a sentence
55. parole
56. probation
57. clemency
58. amnesty
59. recidivism
60. incarceration
61. complicity
62. felony
63. misdemeanor
64. contravene
65. in compliance with
66. oversight
67. stipulate
68. legally binding
69. indemnify
70. probate
71. bequeath
72. unconstitutional
73. judicial review
74. separation of powers
75. checks and balances
76. judiciary
77. recuse
78. gag order
79. contempt of court
80. restraining order
81. cease and desist
82. probable cause
83. exculpatory
84. incriminate
85. defamation
86. libel
87. restitution
88. dissenting opinion
89. lodge a complaint
90. grant bail
91. the letter of the law
92. prima facie
93. litigious
94. culpable
95. enjoin
96. remand
97. absolve
98. appellant
99. amicus curiae
100. motion to dismiss

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-526-600/007` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
