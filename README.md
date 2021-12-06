# HDD
Heart Disease AI Datathon, 심초음파/심전도 ai 모델 데이터톤 2021

## 한우정과 아이들 팀

### 실행 가이드
1. ```test.ipynb```open
2. data가 존재하는 path 설정
3. ```<Set Dataset>```, ```<DataLoader>``` 진행
4. ```<Model Load>``` 내에 저장된 ```my_model_A2C```와 ```my_model_A4C```을 불러옴
  
```python
model_a2c = tf.keras.models.load_model('''my_model_A2C 폴더가 존재하는 dir''')
model_a4c = tf.keras.models.load_model('''my_model_A4C 폴더가 존재하는 dir''')
```

5. ```<Evaluate>``` loss Function 확인
6-1. ```<A2C Evaluate>``` DSC/JI 값 확인 
6-2. ```<A4C Evaluate>``` DSC/JI 값 확인
