# 2단계 — TEPS 입문 004권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-000-326/unit-004.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-000-326` (~326, 입문) · unit 004 · 테마: 교통과 여행 — 예약·길찾기·지연
- 밴드 성격: 3+급 이하. 일상·캠퍼스 대화의 구어 표현과 고등학교 수준 기본 어휘. 텝스 청해 Part 1-2와 어휘 Part 1 대화 완성에 나오는 말.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-000-326-u004
type: voca
level: 1
difficulty: beginner
tags: [teps, vocabulary, unit-004]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-000-326
score_min: 0
score_max: 326
---

# 입문 004권 — 교통과 여행 — 예약·길찾기·지연

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
1. travel
2. trip
3. tour
4. journey
5. vacation
6. book
7. reservation
8. check in
9. check out
10. passport
11. visa
12. ticket
13. round-trip
14. one-way
15. fare
16. seat
17. aisle seat
18. window seat
19. boarding pass
20. board
21. gate
22. flight
23. airport
24. departure
25. arrival
26. land
27. take off
28. delay
29. miss the flight
30. catch a bus
31. get on
32. get off
33. transfer
34. subway
35. station
36. stop
37. platform
38. timetable
39. luggage
40. baggage
41. suitcase
42. pack
43. unpack
44. carry-on
45. lost and found
46. directions
47. ask for directions
48. get lost
49. map
50. turn left
51. go straight
52. corner
53. block
54. cross
55. crosswalk
56. across from
57. next to
58. in front of
59. far
60. nearby
61. distance
62. how far
63. take a taxi
64. give someone a ride
65. drop off
66. traffic
67. traffic jam
68. stuck in traffic
69. rush hour
70. detour
71. route
72. shortcut
73. parking lot
74. gas station
75. drive
76. rent a car
77. driver's license
78. speed limit
79. accident
80. highway
81. exit
82. fasten
83. seat belt
84. hotel
85. stay
86. guest
87. front desk
88. sightseeing
89. tourist
90. guide
91. souvenir
92. abroad
93. overseas
94. foreign
95. local
96. destination
97. itinerary
98. leave for
99. head for
100. set off

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-000-326/004` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
