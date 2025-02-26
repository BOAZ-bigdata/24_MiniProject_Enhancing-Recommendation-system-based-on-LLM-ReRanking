# 24_MiniProject_Enhancing-Recommendation_system_based_on_LLM-ReRanking
LLM을 활용한 추천시스템 개선 프로젝트


##Usage
- [ ] 세션
- [ ] 컨퍼런스
- [X] 미니프로젝트
- [ ] 스터디


<br/>

## Period
### 2025.2.2~2025.2.27


<br/>

## Team 
- PM: [[홍준기](https://github.com/JoonKeeHong00)]
- Team members: [[경재영](https://github.com/economy0)]  ,[[서혜현](https://github.com/hyehyunseo)]  , [[원서현](https://github.com/seohyun126)]


<br/>


## Project Summary
본 Project는 기존 딥러닝 기반 추천시스템에서 나아가, 일부 sample을 대상으로 LLM을 활용하여 추천시스템의 결과를 Re-Ranking하는 과정을 구현하고 기존의 방식을 변경, 수정, 보완하여 추천시스템에서의 LLM의 활용가능성을 탐구하고, 결과를 제언하고자함.
-----------------------------------------------------
### Phase0: Data Load and Preprocessing
- MovieLens_1M dataset의 undersampling 진행
### Phase1: NCF based Recommnedation system Development
- Implicit data(0,1)을 평점(rating threshold>=3)으로 설정하여 진행
- Negative sampling 및 LOO 방식을 통한 Validation 
- 평가지표: Top_10 NDCG+ Hit ratio
> User 별 Recommendation list top_10 도출

### Phase2: Spectral Clustering 
- Graph based clustering을 통한 User representative 및 reference user 도출
> LLM 적용 Representative 도출

### Phase3: LLM Enhanced ReRanking Model Complementation
- 기존 방식에서 수정하여 Similar_user의 특성 반영, Chain-of-thought 방식 구현
> Previous phase에서 도출된 Target_user Recommendation list의 합리성 및 개선점 제언


<br/>

## ETCs
- pandas>=2.0.0
- openai==0.28
- torch>=2.0.0
- numpy>=2.2.0
