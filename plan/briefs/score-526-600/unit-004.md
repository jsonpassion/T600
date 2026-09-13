# 2단계 — TEPS 고급 004권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-526-600/unit-004.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-526-600` (526-600, 고급) · unit 004 · 테마: 국제 관계와 안보 — 분쟁·협정·제재
- 밴드 성격: 1+급. 신문 사설·학술 논문 수준의 고난도 문어 어휘, 미묘한 뉘앙스 형용사·동사, 고난도 콜로케이션과 관용어.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-526-600-u004
type: voca
level: 4
difficulty: advanced
tags: [teps, vocabulary, unit-004]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-526-600
score_min: 526
score_max: 600
---

# 고급 004권 — 국제 관계와 안보 — 분쟁·협정·제재

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
1. territorial integrity
2. incursion
3. encroachment
4. hostilities
5. ceasefire
6. armistice
7. détente
8. rapprochement
9. deterrence
10. proliferation
11. nonaggression pact
12. warhead
13. uranium enrichment
14. blockade
15. retaliation
16. reprisal
17. escalation
18. brinkmanship
19. saber-rattling
20. flashpoint
21. quagmire
22. counterinsurgency
23. guerrilla
24. militia
25. paramilitary
26. junta
27. regime change
28. defector
29. asylum seeker
30. displaced person
31. humanitarian corridor
32. peacekeeping force
33. unilateral
34. bloc
35. entente
36. communiqué
37. memorandum of understanding
38. signatory
39. emissary
40. attaché
41. diplomatic immunity
42. persona non grata
43. hegemony
44. superpower
45. sphere of influence
46. balance of power
47. buffer zone
48. demilitarized zone
49. no-fly zone
50. secession
51. separatist
52. self-determination
53. irredentism
54. isolationism
55. interventionism
56. realpolitik
57. soft power
58. covert operation
59. cyberwarfare
60. proxy war
61. mobilize
62. conscription
63. collateral damage
64. atrocity
65. genocide
66. ethnic cleansing
67. reparations
68. quid pro quo
69. bargaining chip
70. broker
71. mediator
72. shuttle diplomacy
73. back channel
74. stand down
75. pull out
76. deploy
77. garrison
78. reconnaissance
79. airstrike
80. preemptive strike
81. jingoism
82. xenophobia
83. pariah state
84. rogue state
85. failed state
86. client state
87. puppet government
88. destabilize
89. subjugate
90. insurrection
91. clandestine
92. confidence-building measure
93. heightened tensions
94. annexation
95. appeasement
96. nonproliferation
97. bellicose
98. casus belli
99. war of attrition
100. sticking point

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-526-600/004` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
