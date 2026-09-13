# 2단계 — TEPS 중상급 005권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-453-525/unit-005.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-453-525` (453-525, 중상급) · unit 005 · 테마: 문화와 예술 — 비평·전시·공연
- 밴드 성격: 1급. 시사·학술 지문의 문어체 어휘, 격식 표현, 관용어와 다의 구동사. 어휘 Part 2 문장 완성 20문항의 주력 구간.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-453-525-u005
type: voca
level: 3
difficulty: upper-intermediate
tags: [teps, vocabulary, unit-005]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-453-525
score_min: 453
score_max: 525
---

# 중상급 005권 — 문화와 예술 — 비평·전시·공연

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
1. critique
2. acclaim
3. rave review
4. scathing
5. mediocre
6. masterpiece
7. genre
8. aesthetic
9. realism
10. avant-garde
11. contemporary
12. exhibit
13. curator
14. retrospective
15. installation
16. sculpture
17. still life
18. canvas
19. brushstroke
20. palette
21. depict
22. portray
23. evoke
24. convey
25. symbolize
26. allegory
27. metaphor
28. motif
29. narrative
30. protagonist
31. antagonist
32. plot twist
33. climax
34. premiere
35. debut
36. rehearsal
37. audition
38. ensemble
39. composer
40. repertoire
41. virtuoso
42. recital
43. concerto
44. symphony
45. choreography
46. playwright
47. screenplay
48. blockbuster
49. standing ovation
50. encore
51. intermission
52. stage fright
53. steal the show
54. bring the house down
55. spectator
56. patron
57. commission
58. prolific
59. renowned
60. versatile
61. originality
62. authenticity
63. replica
64. restoration
65. heritage
66. folklore
67. indigenous
68. multicultural
69. mainstream
70. subculture
71. highbrow
72. lowbrow
73. cult following
74. censorship
75. controversial
76. subversive
77. satire
78. parody
79. irony
80. nuance
81. subtle
82. vivid
83. expressive
84. interpret
85. reminiscent of
86. draw inspiration from
87. muse
88. improvise
89. verse
90. stanza
91. prose
92. anthology
93. memoir
94. literary
95. nonfiction
96. bestseller
97. manuscript
98. edition
99. artisan
100. craftsmanship

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-453-525/005` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
