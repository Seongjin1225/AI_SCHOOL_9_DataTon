# AI_SCHOOL_9_DataTon
AI School 9기 데이터톤 
# 주제
- 숫자 이미지 분류 모델 개발
# 진행 과정
- 1. 학습에 필요한 숫자 데이터 수집
  2. 이미지 숫자 인식 모델 구현
  3. 정확도 측정
  4. 기술의 방향성 제시
# 평가 방식
- 모델의 최종 평가는 제공되는 테스트 데이터셋과 유사한 이미지로 평가 
- 이 최종 평가를 위한 데이터셋은 따로 제공되지 않음
- 모델 구현이 끝나고 구현된 모델을 제출한 후 최종 평가 데이터셋을 이용하여 모델을 평가
- 평가 기준은 Accuracy

# 사용 데이터
- Stanford Univ.에서 제공한 SVHN(Street View House Number) 데이터
- HuggingFace에 올라온 가공된 버전의 데이터를 이용
- Train : 73,257
- Test : 26,032
- Test set의 20%를 validation에 사용

![svhn](https://github.com/Seongjin1225/AI_SCHOOL_9_DataTon/assets/114036940/68b17cb2-87e7-4216-852e-010b8a6dd476)

# 기반 모델(DenseNet)
![densenet](https://github.com/Seongjin1225/AI_SCHOOL_9_DataTon/assets/114036940/212828c0-16ec-409d-95df-627b35d4e247)
- DenseNet은 모든 레이에의 feature map을 연결한다는 특징 존재
- 즉, 이전 레이어의 featur map 그 이후의 모든 레이어의 featrue map에 연결
- 파라미터 수와 연산량이 적다는 장점 존재
