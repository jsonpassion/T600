# 2단계 — TEPS 입문 010권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-000-326/unit-010.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-000-326` (~326, 입문) · unit 010 · 테마: 여가와 미디어 — 영화·운동·취미
- 밴드 성격: 3+급 이하. 일상·캠퍼스 대화의 구어 표현과 고등학교 수준 기본 어휘. 텝스 청해 Part 1-2와 어휘 Part 1 대화 완성에 나오는 말.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-000-326-u010
type: voca
level: 1
difficulty: beginner
tags: [teps, vocabulary, unit-010]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-000-326
score_min: 0
score_max: 326
---

# 입문 010권 — 여가와 미디어 — 영화·운동·취미

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
1. free time
2. spare time
3. hobby
4. leisure
5. movie
6. film
7. see a movie
8. theater
9. box office
10. actor
11. actress
12. director
13. main character
14. plot
15. scene
16. ending
17. spoiler
18. sequel
19. horror movie
20. comedy
21. action movie
22. documentary
23. drama
24. romantic comedy
25. cartoon
26. animation
27. subtitle
28. dubbed
29. rating
30. must-see
31. boring
32. exciting
33. entertaining
34. touching
35. scary
36. hilarious
37. episode
38. series
39. channel
40. binge-watch
41. stream
42. subscribe
43. program
44. broadcast
45. host
46. audience
47. fan
48. celebrity
49. famous
50. concert
51. song
52. singer
53. band
54. album
55. musical
56. play
57. exhibition
58. museum
59. gallery
60. draw
61. photography
62. take pictures
63. camera
64. novel
65. magazine
66. comic book
67. video game
68. board game
69. puzzle
70. work out
71. gym
72. jog
73. swim
74. go hiking
75. camping
76. fishing
77. soccer
78. baseball
79. basketball
80. yoga
81. player
82. coach
83. win
84. lose
85. tie
86. cheer for
87. root for
88. compete
89. tournament
90. practice
91. get in shape
92. out of shape
93. take up
94. be into
95. be crazy about
96. kill time
97. chill out
98. relax
99. have fun
100. weekend

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-000-326/010` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
