# CheXNet

Kaggle에 있는 NIH Chest X-ray 데이터셋을 사용해 흉부 X-ray 영상의 다중 레이블 분류 모델인 CheXNet을 구현하고, Grad-CAM을 활용해 모델의 예측 근거를 시각화하였습니다.

## Implementations

### 1. CheXNet-Baseline
- 흉부 X-ray 영상 기반 다중 레이블 분류
- 14개 질환 레이블 예측

### 2. CheXNet-GradCAM
- Grad-CAM을 활용한 모델의 주요 관심 영역 시각화
- 클래스별 예측 결과에 대한 해석 가능성 분석

## Setting
- DenseNet121 torchvision 구현체 사용
- 환자 단위 데이터 분할(Patient-level split)을 통해 학습 데이터와 검증 데이터 간 환자 중복 방지

## Dataset
- [NIH Chest X-rays(kaggle)](https://www.kaggle.com/datasets/nih-chest-xrays/data)

## Blog
- [CheXNet 구현, 리뷰](https://icedtea.tistory.com/entry/%EB%A6%AC%EB%B7%B0CheXNet-Radiologist-Level-Pneumonia-Detection-on-Chest-X-Rays-with-Deep-LearningarXiv-preprint-2017)

## References
- [CheXNet: Radiologist-Level Pneumonia Detection on Chest X-Rays with Deep Learning](https://arxiv.org/abs/1711.05225)
