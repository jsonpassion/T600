# 2단계 — TEPS 중급 004권 작성

너는 텝스(TEPS) 어휘 교재 저자다. 아래 **배정된 100개 표제어만** 사용해 앱이 읽는 단어책 파일 하나를
`content/voca/score-327-452/unit-004.md`에 쓴다. 표제어를 바꾸거나 빼거나 더하지 않는다 — 다른 권과의 중복은 이미 제거되어 있다.

## 이 권
- band_id `score-327-452` (327-452, 중급) · unit 004 · 테마: 기술과 인터넷 — 기기·보안·서비스
- 밴드 성격: 2급·2+급(국가공인 진입). 비즈니스·사회 전반의 빈출 어휘, 기본 콜로케이션과 구동사. 서울대 대학원 최소 기준 327점을 넘기는 구간.

## 파일 형식 — 한 글자도 다르지 않게
```
---
id: voca-327-452-u004
type: voca
level: 2
difficulty: intermediate
tags: [teps, vocabulary, unit-004]
source: t600
version: 1
updated_at: 2026-09-14T00:00:00Z
score_band_id: score-327-452
score_min: 327
score_max: 452
---

# 중급 004권 — 기술과 인터넷 — 기기·보안·서비스

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
1. device
2. gadget
3. laptop
4. hardware
5. software
6. download
7. install
8. uninstall
9. upgrade
10. outdated
11. obsolete
12. compatible
13. user-friendly
14. interface
15. feature
16. malfunction
17. glitch
18. bug
19. crash
20. reboot
21. shut down
22. boot up
23. log in
24. log out
25. two-factor authentication
26. verify
27. encryption
28. hacker
29. hack into
30. data breach
31. malware
32. computer virus
33. spam
34. phishing
35. firewall
36. antivirus software
37. back up
38. cloud storage
39. storage capacity
40. network
41. wireless
42. bandwidth
43. broadband
44. streaming
45. unsubscribe
46. social media
47. browser
48. search engine
49. click on
50. scroll down
51. navigate
52. bookmark
53. cookie
54. privacy setting
55. personal information
56. identity theft
57. surveillance
58. tech-savvy
59. digital
60. digitize
61. artificial intelligence
62. algorithm
63. automate
64. virtual reality
65. innovation
66. cutting-edge
67. state-of-the-art
68. breakthrough
69. prototype
70. release
71. battery life
72. charger
73. unplug
74. switch off
75. touchscreen
76. troubleshoot
77. technical support
78. portable
79. wearable
80. sensor
81. delete
82. restore
83. access
84. gain access to
85. unauthorized
86. vulnerability
87. secure
88. security patch
89. go viral
90. e-commerce
91. cashless
92. mobile payment
93. contactless
94. screen time
95. cyberattack
96. cybersecurity
97. misinformation
98. specification
99. processor
100. operating system

## 저장 전 스스로 확인
① 100줄인가 ② 모든 줄이 6필드인가 ③ 배정표와 표제어가 정확히 같은가 ④ IPA가 `/…/`인가
⑤ TIP이 45자 이내이고 뜻의 반복이 아닌가 ⑥ 예문에 표제어가 들어 있는가.
저장 후 `python3 tools/validate_content.py --unit score-327-452/004` 를 실행해 0 errors가 될 때까지 해당 줄만 고친다.
