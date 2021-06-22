
<광고배너 pCTR 예측하기>
0. 카카오 기술 블로그 : https://brunch.co.kr/@kakao-it/84
- 추천시스템과 CTR 예측은 분리할 수 없다. 

1. DeepFM 논문 리뷰 및 파이프라인 구현 
논문 리뷰: https://greeksharifa.github.io/machine_learning/2020/04/07/DeepFM/

코드 : https://github.com/ChenglongChen/tensorflow-DeepFM
- 전처리과정이 필요없다고 한다. 
- 이걸 이해하려면 FM도 이해해야한다. FM 개념 및 영화 추천 필사 해보기
- 메모리 문제 있음, 카테고리컬 컬럼은 값이 천이 넘어가면 메모리 156기가에서도 안돌아간다. 


2. python xlearn 라이브러리  -> https://xlearn-doc.readthedocs.io/en/latest/python_api/

* 번개장터 기술블로그 참고 : https://www.kgsbdata.com/post/ctr%EC%9D%84-%EC%98%88%EC%B8%A1%ED%95%98%EB%8A%94-%EA%B8%B0%EC%88%A0-3-factorization-machine
- 가성비가 좋은 모델이라고 함.

3. 다 안되면, 기존 코드로 텐서플로우로 코드 재설계
- 기존에 버스 도착 시간 예측 때 사용한 코드 사용 

4. 베이스라인 코드인 LightGBM 모델 공부 
5. 
- LGBM 성능 높이는 법 
6) Aggregation , 특정 변수의 mean , std , max, min 값 등을 변수로 추가
7) 카테고리컬 변수 지정
8) 편향된 테스트 셋에 보정?
