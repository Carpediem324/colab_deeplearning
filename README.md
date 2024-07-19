# Google Colab으로 배우는 머신러닝


## 0. Google Colab 사용하기

AI, 딥러닝이 핫하다고는 하는데...

뭐부터 준비해야하지? 해서 시작한 프로젝트 

- 고성능 GPU 탑재 PC
- CUDA 설치 및 세팅
- 개념서

일단 google colab으로 말로만 하지말고 간단하게 파이토치 텐서플로우 구현해보자!

https://colab.research.google.com/

### Colab이란?

Colaboratory(줄여서 'Colab'이라고 함)을 통해 브라우저 내에서 Python 스크립트를 작성하고 실행할 수 있습니다.
- 구성이 필요하지 않음
- 무료로 GPU 사용
- 간편한 공유

## 1. 그래서 어떻게 시작하게?

한국어로 수업듣는게 가장 편하게 배울 수 있는 방법이니 모교의 온평원을 이용해보자...


https://www.step.or.kr/

[K-디지털] 머신러닝 실습을 위한 Google Colab 활용

하지만 바쁜 현대인이니 거를건 거르면서 듣자..

구글 코랩은 조금 만져보면 알만한 파이썬. PASS

```python
 # 플랫폼 보기
import platform
platform.platform() 

# CPU 모델 이름
!lsCPU | grep 'Model name'

# CPU 사양
!cat /proc/cpuinfo

# 사용가능 메모리
!free -h --si | awk '/Mem:/{print $2}'

# 사용가능 하드 디스크 용량
!df -h / | awk '{print $4}'

# GPU 갯수와 이름 #에러가 나는 경우는 런타임 >> 런타임 유형 변경 >> 하드웨어 가속기에 GPU선택
!nvidia-smi -L
```



# 