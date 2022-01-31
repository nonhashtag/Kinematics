# Kinematics
Dataset by M Yasser H (Kaggle)

https://www.kaggle.com/yasserh/kinematics-motion-data



## Target Data

### 1. wrist
#### - 0 : left wrist
#### - 1 : right wrist

</br>

### 2. activity
#### - 0 : walking
#### - 1 : running

</br>

</br>

## EDA (Exploratory Data Analysis)
### - 불균형 확인
### - 결측치 확인
### - 속성간 상관관계 확인
### - 차원축소(PCA, TSNE)
##### (차원축소 추가중)


## Model
### LGBM
#### 학습데이터 분할 : train 7, test 3
#### 교차검증 : Stratified, K-Fold
#### 하이퍼 파라미터 학습 : GridSearch
#### 성능 평가 : confusion_matrix
- Accuracy
- Recall
- Precision
- F1 score
