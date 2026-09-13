# 2단계 — TEPS 중급 008권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-327-452/unit-008.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-327-452` (327-452, 중급) · unit 008 · 테마: 감정과 인간관계 — 갈등·화해 구동사
- 밴드 성격: 2급·2+급(국가공인 진입). 비즈니스·사회 전반의 빈출 어휘, 기본 콜로케이션과 구동사. 서울대 대학원 최소 기준 327점을 넘기는 구간.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-327-452-u008
type: voca
level: 2
difficulty: intermediate
tags: [teps, vocabulary, unit-008]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-327-452
score_min: 327
score_max: 452
---

# 중급 008권 — 감정과 인간관계 — 갈등·화해 구동사

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
1. make up with
2. patch up
3. kiss and make up
4. bury the hatchet
5. fall out with
6. split up
7. drift apart
8. grow apart
9. get along with
10. hit it off
11. get on someone's nerves
12. rub someone the wrong way
13. pick a fight
14. pick on
15. lash out
16. blow up
17. flare up
18. calm down
19. cool off
20. let off steam
21. hold a grudge
22. hold it against
23. forgive and forget
24. owe someone an apology
25. make amends
26. reconcile
27. resentment
28. take offense
29. hurt someone's feelings
30. get even with
31. take it out on
32. talk back
33. put down
34. look down on
35. look up to
36. stand by
37. stick up for
38. side with
39. turn against
40. turn one's back on
41. let down
42. walk out on
43. cut off
44. give someone the cold shoulder
45. stab someone in the back
46. betray
47. trustworthy
48. count on
49. confide in
50. open up
51. talk things over
52. clear the air
53. sort out
54. smooth over
55. come around
56. give in
57. back down
58. stand one's ground
59. agree to disagree
60. at odds with
61. on good terms
62. bad blood
63. tension
64. friction
65. quarrel
66. bicker
67. confront
68. hostile
69. jealous
70. envy
71. annoyed
72. irritated
73. furious
74. heartbroken
75. isolated
76. awkward
77. guilt
78. regret
79. sympathize
80. empathy
81. compassion
82. considerate
83. sensitive
84. insult
85. blame
86. point the finger at
87. gossip
88. spread a rumor
89. intermediary
90. misunderstanding
91. take it the wrong way
92. no hard feelings
93. let bygones be bygones
94. turn over a new leaf
95. get over
96. move on
97. bounce back
98. console
99. reassure
100. lose touch

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-327-452/008` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
