# Bike Shring Demand 

---

-  data: https://www.kaggle.com/c/bike-sharing-demand

## BSD_EDA

Load Data,  (중복, 결측, datetime), 시각화 순으로 진행함

하루 중 출퇴근 시간인 8시와 17-18시에 대여량이 가장 많습니다. 사람들이 출퇴근하면서 자전거를 많이 대여하는 모양입니다. 하지만 이는 주중에 주로 나타나는 특성입니다. 주말에는 8시, 17-18시보다는 오후 시간대에 대여량이 많았습니다. 주중엔 출퇴근 시간, 주말엔 오후 시간대에 대여량이 많습니다. 주중은 5일이고, 주말은 2일이므로 이 둘을 합치면 8시, 17-18시에 대여량이 많아 보이게 됩니다.

계절별로는 여름에 대여량이 많습니다. 아무래도 날씨가 추울 때보단 따뜻하거나 더울 때 더 많이 타는 것 같습니다. 또한 2011년보다 2012년에 사용자가 더 많습니다.

## BSD by Random Forest

Missing Value를 머신러닝을 통해 채웠습니다. Missing Value를 채우는 가장 기본적인 방법은 평균값으로 채워주는 것입니다. 하지만 Missing Value 자체를 Target Value라 생각하고 다른 데이터를 활용해 예측해줄 수도 있습니다. Missing Value 이외의 데이터를 살아있으니 살아있는 데이터를 Feature라 생각하고, 해당 Feature를 기반으로 모델을 학습시켜 Missing Value를 예측해주는 것입니다. 이런 식으로 예측해 Missing Value를 채워주면 단순히 평균값으로 예측하는 것보다 더 정확히 예측할 수 있습니다.

## BSD by Ensemble