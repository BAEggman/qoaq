# qoaq 배포 진행 기록

## 2026-07-22

### 인출훈련 SRS 배포 — `한의학_인출훈련_학습과학.html`

- 배포 파일: `한의학_인출훈련_학습과학.html` (qoaq 루트, 신규 추가)
- 배포 URL: https://baeggman.github.io/qoaq/한의학_인출훈련_학습과학.html
- 커밋 해시: `934f46a47e0bf5b8edc597b1abff8b5cd52cda5c` (`934f46a`)
- 진도 KEY: `hanui_retrieval_v1` (origin baeggman.github.io 공유 → 진도 유지)

변경 요약
- 선지 소실 21장 복원: 선지 13장(HUBJQ-0149~0154, HUBGR-0059·0060·0144~0147·0173) + 함정 9유형 목록 8장(HUBJQ-0155~0162)
- `.qtext white-space:pre-line` 추가(선지 줄바꿈 렌더)
- feat: 그날 틀린 문제 → 세뇌 암기송 프롬프트 생성(collectWrong/buildSongPrompt/openSongModal, 세션종료 버튼)
- 과적재 34장 → 세트 앵커(슬림화) + 항목별 원자 122장 추가(1894→2016)
- CSV 불러오기 버튼 라벨 1894 → 2016 갱신

검증 결과 수치
- 카드 수 **2016장** · 과목 **13종** · 빈 필드 **0** · 빈 exp.logic **0** · id 중복 **0**
- 선지 소실 재발 **0** · localStorage 키 동일(`hanui_retrieval_v1`) · 기존 id 소실 **0** (직전 1894장 대비 신규 122장)
- 외부 의존성 **0** (자기완결 단일 파일)

미해결(교재 대조 필요·※)
- 장 배속 재검토 3건: OHG2-010 · OHG2-001 · OHG-043/BGI-SA-06
- 정답해설 원문오류 1건: 정기신혈진액 3차분 Q148(氣脫者耳聾 ↔ 精脫者目不明)
- 2항목 카드 추가 분해 보류 3장: JQ-JEONG-07 · BIN-EO-02 · BGI-JIN-01
