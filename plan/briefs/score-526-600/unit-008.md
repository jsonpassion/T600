# 2단계 — TEPS 고급 008권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-526-600/unit-008.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-526-600` (526-600, 고급) · unit 008 · 테마: 언론과 수사 — 논조·풍자·비판
- 밴드 성격: 1+급. 신문 사설·학술 논문 수준의 고난도 문어 어휘, 미묘한 뉘앙스 형용사·동사, 고난도 콜로케이션과 관용어.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-526-600-u008
type: voca
level: 4
difficulty: advanced
tags: [teps, vocabulary, unit-008]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-526-600
score_min: 526
score_max: 600
---

# 고급 008권 — 언론과 수사 — 논조·풍자·비판

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
1. editorial
2. op-ed
3. polemic
4. diatribe
5. invective
6. philippic
7. tirade
8. screed
9. harangue
10. lampoon
11. satirize
12. pastiche
13. caricature
14. burlesque
15. travesty
16. sardonic
17. acerbic
18. caustic
19. mordant
20. trenchant
21. withering
22. vitriolic
23. barbed
24. excoriate
25. castigate
26. lambaste
27. pillory
28. censure
29. decry
30. vilify
31. ridicule
32. derision
33. scorn
34. sarcasm
35. hyperbole
36. understatement
37. litotes
38. euphemism
39. innuendo
40. insinuation
41. allusion
42. rhetorical question
43. oratory
44. eloquence
45. bombast
46. grandiloquent
47. florid
48. turgid
49. verbose
50. pithy
51. purple prose
52. platitude
53. bromide
54. cliché
55. demagogue
56. mouthpiece
57. spin doctor
58. sensationalism
59. yellow journalism
60. tabloid
61. muckraker
62. exposé
63. scoop
64. byline
65. masthead
66. pundit
67. columnist
68. correspondent
69. off the record
70. on condition of anonymity
71. fact-check
72. disinformation
73. slant
74. tendentious
75. even-handed
76. editorialize
77. loaded language
78. sound bite
79. talking point
80. framing
81. agenda-setting
82. gatekeeping
83. press freedom
84. self-censorship
85. issue a retraction
86. smear campaign
87. character assassination
88. hatchet job
89. distort
90. misrepresent
91. quote out of context
92. cherry-pick
93. verbatim
94. tongue-in-cheek
95. deadpan
96. wry
97. droll
98. irreverent
99. backhanded compliment
100. come under fire

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-526-600/008` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
