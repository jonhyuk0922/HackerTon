LightGBM 

- 공식문서 : https://lightgbm.readthedocs.io/en/latest/index.html

- 목적 : 모델의 장단점 , 하이퍼 파라미터 , 사용법 및 코드 예제, 구동원리 이해 , 

<h3>0.LGBM 이란?</h3>
![스크린샷 2021-06-24 오후 11 01 50](https://user-images.githubusercontent.com/76195885/123276472-2a588680-d540-11eb-9d4c-2a55dddaacfa.png)

- 트리 기반의 학습 알고리즘인 gradient boosting 방식의 프레임 워크다. 
- 같은 부스팅 방식인 XG Boost 방식(Level-wise tree growth)과 달리,
(Leaf-wise tree growth) 트리의 균형을 맞추지 않고 최대 손실값을 가지는 leaf node를 지속적으로 분할하면서 트리의 깊이가 깊어져 비대칭 트리가 생긴다. 이렇게 지속적으로 분할해 예측 오류 손실을 최소화 한다.


<h3>1. 모델의 장단점</h3>

- 장점 
: 우선 Light라는 이름처럼 학습이 빠르고 메모리 사용량도 적다. 데이터가 많아지는 요즘에 적합한 모델이다. 
: 또한, 카테고리형 피처의 자동 변환과 최적 분할이 가능하다. 원핫 인코딩 없이도 최적으로 변환하고 이에 따른 노드 분할을 수행한다.
- 단점 
: 다른 트리에 비해 과대적합에 민감하다. 10000개 이하의 데이터에서는 사용이 권장되지 않는다.


<h3>2. 하이퍼 파라미터</h3>
![스크린샷 2021-06-24 오후 10 58 23](https://user-images.githubusercontent.com/76195885/123275905-aef6d500-d53f-11eb-921a-db7a8756ba4e.png)




<h4>Reference</h4>
https://greatjoy.tistory.com/72
https://databoom.tistory.com/entry/LightGBM%EC%84%A4%EB%AA%85
https://ariz1623.tistory.com/209
https://greeksharifa.github.io/machine_learning/2019/12/09/Light-GBM/
https://nicola-ml.tistory.com/51
https://nurilee.com/2020/04/03/lightgbm-definition-parameter-tuning/
