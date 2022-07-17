# Python_optimization

## python -m cProfile ~~.py
- 파이썬 실행시간 분석
## ![image](https://user-images.githubusercontent.com/54635552/179389303-baa43538-c93f-423c-a08e-0919dd5de382.png)

## third-party 패키지
- PyPy : 파이썬 코드 최적화 하기위한 JIT 컴파일러
- Cython : Python 코드 C로 변환
- ShedSkin : Python 코드 C++로 변환
- GPULib : 코드의 속도향상을 위해 GPU 사용

## Multiprocessing Module 사용
- GIL(Global Interpreter Lock) : 파이썬에서 하나의 프로세스 안에 모든 자원을 Lock을 Global하게 관리하므로, 한번에 한개의 Thread만 자원을 컨트롤하여 동작
- 동시에 여러개 쓰레드 실행시켜도 GIL 떄문에 한번에 하나의 쓰레드만 계산을 진행함
- Python에선 멀티 쓰레드보다 멀티 프로세스를 사용하는것이 효율적
- 싱글 머신 아키텍처로부터 여러 머신을 사용하는 분산 애플리케이션으로 전환하기쉬움, 쓰레드에 비해 메모리 사용량이 늘어남


## JIT 사용
- 프로그램 실행 속도를 빠르게하기위해, 프로그램 실제 실행하는 시점에서 기계어로 번역하는 컴파일 기법
- PyPy, Numba, Cython 존재
