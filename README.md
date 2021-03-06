# GAN_Study
GAN에 대해 공부하고 직접 모델을 구축하여 학습시켜봄.

## DCGAN
DCGAN은 스스로 학습하고 의미 있는 이미지를 생성하는 GAN 모델을 구축하는 방법을 소개한 GAN 초기 모델 중 하나이다.

관련 논문은 [https://arxiv.org/pdf/1511.06434.pdf](https://arxiv.org/pdf/1511.06434.pdf) 에서 찾아볼 수 있다.

DCGAN.ipynb에서는 위의 논문에서 소개된 DCGAN을 기초로 GAN 아키텍처를 훈련시키는 여러 부분을 구현해본다.

## DCGAN 학습에 필요한 요소는 다음과 같다.

* 생성기 네트워크 : 생성기 네트워크는 고정된 차원의 잠재 벡터를 어떤 형상의 이미지에 대응시킨다.
* 판별기 네트워크 : 생성기 네트워크가 만든 이미지 또는 실제 데이터셋의 이미지를 입력받는다. 그리고 이미지가 실제인지 가짜인지 평가 점수를 출력한다.
* 생성기와 판별기를 위한 오차 함수 정의
* 옵티마이저 정의
* GAN 학습

