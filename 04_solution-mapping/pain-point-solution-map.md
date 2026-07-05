# Pain Point → Digital/AI 솔루션 매핑

## 매핑 테이블

| Pain Point | 제안 솔루션 | 핵심 기술 | 왜 이 솔루션인가 |
|---|---|---|---|
| PP1. 육안검사 의존에 따른 검출률 편차 | Vision AI 기반 자동 외관검사 | Computer Vision (딥러닝 이미지 분류/객체탐지) | 검사자 편차를 제거하고 24시간 일관된 기준 적용 가능. M-SPHERE에서 이미 비전검사 기술을 공개한 만큼 회사 방향과 부합 |
| PP2. 검사 결과 데이터 파편화 | 검사 데이터 표준화 + 통합 대시보드 | Data Pipeline(ETL) + BI Dashboard | 라인/공정별 흩어진 데이터를 하나의 스키마로 통합해야 이후 분석·AI 적용의 기반이 됨. 모든 AI 솔루션의 전제조건 |
| PP3. 불량 원인 분석 및 라인 피드백 지연 | 실시간 이상탐지 + 자동 알림 | Anomaly Detection + Rule-based Alert / RPA 연동 | 원인분석 대기시간을 줄여 재작업 사이클 타임 단축. PP2(데이터 통합) 이후에 적용 가능한 후속 단계 |

## 우선순위 매트릭스 (Impact vs Feasibility)

​```mermaid
quadrantChart
    title Pain Point 우선순위
    x-axis Low Feasibility --> High Feasibility
    y-axis Low Impact --> High Impact
    quadrant-1 Quick Win
    quadrant-2 Strategic Bet
    quadrant-3 Deprioritize
    quadrant-4 Fill-in
    "PP2 데이터 표준화": [0.75, 0.65]
    "PP1 Vision AI 검사": [0.45, 0.85]
    "PP3 실시간 이상탐지": [0.35, 0.6]
