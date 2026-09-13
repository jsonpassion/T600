# 2단계 — TEPS 고급 002권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-526-600/unit-002.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-526-600` (526-600, 고급) · unit 002 · 테마: 고급 동사 — 격식체 동사와 완곡 표현
- 밴드 성격: 1+급. 신문 사설·학술 논문 수준의 고난도 문어 어휘, 미묘한 뉘앙스 형용사·동사, 고난도 콜로케이션과 관용어.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-526-600-u002
type: voca
level: 4
difficulty: advanced
tags: [teps, vocabulary, unit-002]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-526-600
score_min: 526
score_max: 600
---

# 고급 002권 — 고급 동사 — 격식체 동사와 완곡 표현

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
1. ameliorate
2. mitigate
3. assuage
4. allay
5. placate
6. mollify
7. appease
8. obviate
9. preclude
10. forestall
11. avert
12. circumvent
13. eschew
14. forgo
15. relinquish
16. abdicate
17. renounce
18. repudiate
19. disavow
20. recant
21. retract
22. rescind
23. countermand
24. supersede
25. supplant
26. usurp
27. arrogate
28. commandeer
29. procure
30. garner
31. glean
32. amass
33. accrue
34. augment
35. bolster
36. buttress
37. vindicate
38. exonerate
39. condone
40. countenance
41. acquiesce
42. accede
43. capitulate
44. succumb
45. demur
46. balk
47. cavil
48. quibble
49. deprecate
50. disparage
51. denigrate
52. deride
53. chastise
54. admonish
55. reprimand
56. rebuke
57. berate
58. extol
59. laud
60. venerate
61. emulate
62. obfuscate
63. equivocate
64. prevaricate
65. dissemble
66. feign
67. beguile
68. cajole
69. wheedle
70. inveigle
71. elicit
72. engender
73. precipitate
74. instigate
75. foment
76. galvanize
77. impel
78. coerce
79. browbeat
80. expedite
81. rectify
82. redress
83. remunerate
84. recompense
85. impart
86. divulge
87. intimate
88. allude
89. surmise
90. ascertain
91. discern
92. promulgate
93. disseminate
94. burgeon
95. dwindle
96. wane
97. abate
98. subside
99. languish
100. flounder

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-526-600/002` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
