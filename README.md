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
![image](https://user-images.githubusercontent.com/75101880/152645447-6a032c7f-e3c2-4032-a930-08aed479dd26.png)
![image](https://user-images.githubusercontent.com/75101880/152645455-b0289082-be10-4573-b29b-e0a5f4c683f1.png)
</br>
### - 결측치 확인 
- 결측치 없음

</br>

### - 속성간 상관관계 확인
![image](https://user-images.githubusercontent.com/75101880/152645415-74cbbfcf-f907-45f0-a3b4-b05babea9cbd.png)

</br>

### - 차원축소 : PCA, t-SNE (TSNE가 다소 오래걸림)
- 2차원
- 3차원


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

## 결과
### Wrist 예측
Confusion Matrix </br>
[[13674   204] </br>
 [  211 12488]]

Accuracy : 0.9843849945441547 </br>
Recall : 0.9853004755728492 </br>
precision : 0.9848037450486136 </br>
F1 : 0.9850520476893707 </br>
### Activity 예측
Confusion Matrix </br>
[[13149   161] </br>
 [   93 13174]] </br>

Accuracy : 0.9904428641306393 </br>
Recall : 0.9879038317054846 </br>
precision : 0.9929768917082011 </br>
F1 : 0.9904338656221753 </br>

### 테스트 결과 준수한 편이다
