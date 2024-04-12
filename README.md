# 딥러닝을 이용한 반려견 감정 분류 앱 개발
![image](https://github.com/SungChiWoong/Capstone-Design/assets/123548388/a39288f5-3543-45d9-bd20-9ce504e155e2)
> 

## 활동
- 약 1만장의 이미지 데이터 라벨링
- Python을 이용
- Yolov5로 이미지 분류 모델 제작
- LSTM-FCN을 이용하여 강아지 음성 분류 모델 제작
- 두 모델을 합쳐 타 여러 분류 대표 모델(RF, SVM 등)을 비교하여 선정된 MLP를 이용해 최종
적으로 여러개의 감정 중 하나로 분류되도록 설계
- 해당 모델을 REST API를 이용하여 API 제작
- Android Studio에서 코틀린를 이용하여 앱에서 작동할 수 있도록 제작

## 목차
1. 고려 사항
2. Model
  <br>2-1. 영상 Model
  <br>2-2. 음성 Model
  <br>2-3. 분류 Model
3. Application

# 고려사항
1) 목적
  * 반려견이 무슨 생각을 하는지 궁금할 때 간단한 촬영으로 심리상태를 알아봅니다.

2) 아이디어
*  강아지 감정 자채를 Labeling 하는게 맞는가?
<br>![image](https://github.com/SungChiWoong/Capstone-Design/assets/123548388/5e4b226e-4b97-4314-87bc-ee9e0e271523)

* 이미 있는 방법이고 너무 간단하기에, 다른 방법을 모색
* 도메인지식을 찾아본 결과, 강아지의 몸 상태(입, 귀, 꼬리 등), 그리고 음성을 통해 강아지 감정을 분석하는 것을 확인
* 해당 방법을 활용해 만들기로 결정
<br>![image](https://github.com/SungChiWoong/Capstone-Design/assets/123548388/9e3035e7-4cfe-41f5-9f0b-56125d2711e5)





### 참조 : https://github.com/ultralytics/yolov5
