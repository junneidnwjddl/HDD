# HDD
Heart Disease AI Datathon, 심초음파/심전도 ai 모델 데이터톤 2021

## 한우정과 아이들 팀
- **팀장:  [장성준](https://github.com/junnei)**
- 팀원: [한우정](https://github.com/dnwjddl)

### 실행 가이드
1. ```test.ipynb```open
2. data가 존재하는 path 설정
3. ```<Set Dataset>```, ```<DataLoader>``` 진행 / Inference 만을 위해서는 모델 학습 부분 건너뛰어도 무방함
4. ```<Model Load>``` 내에 저장된 ```my_model_A2C```와 ```my_model_A4C```을 불러옴
  
```python
model_a2c = tf.keras.models.load_model('''my_model_A2C 폴더가 존재하는 dir''')
model_a4c = tf.keras.models.load_model('''my_model_A4C 폴더가 존재하는 dir''')
```

5. ```<Evaluate>``` loss Function 확인
6-1. ```<A2C Evaluate>``` DSC/JI 값 확인 
6-2. ```<A4C Evaluate>``` DSC/JI 값 확인

### 환경
- Colab 환경(2021.12.07기준) + tensorflow-addons

### 모델 weight
- Not provided

### 학습코드
[Train-A2C 학습 코드 클릭](https://github.com/junneidnwjddl/HDD/blob/main/Train_u_net_A2C.ipynb)  
[Train-A4C 학습 코드 클릭](https://github.com/junneidnwjddl/HDD/blob/main/Train_u_net_A4C.ipynb)

## Results

- A2C Model Metrics

  - DSC(Dice Similarity Coefficient) : 0.9372626568114139

  - JI(Jaccard Index) : 0.8845628916479535

- A4C Model Metrics

  - DSC(Dice Similarity Coefficient) : 0.9546604165557122

  - JI(Jaccard Index) : 0.914575115481054

