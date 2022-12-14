## Week 5
- CISC와 RISC
- 1,2,3,4,5 단원 복습

## 우성

### 중요
### 문제
### 답

## 하은

### 중요

- CPU 제조사가 여러개인 만큼 CPU가 이해하고 실행하는 명령어는 조금씩 차이가 있다. 이 때 CPU가 이해할 수 있는 명령어들의 모음을 명령어 집합(Instruction set), 명령어 집합 구조(Instruction Set Architecture, ISA)라고 한다. 즉 CPU마다 ISA가 다를 수 있다.
- ISA가 다르면 제어장치가 명령어를 해석하는 방식, 사용하는 레지스터의 종류, 갯수, 메모리 관리 방법 등이 달라진다. 대표적인 현대 ISA에는 CISC와 RISC가 있다.

#### CISC: Complex Instruction Set Computer
- **Complex**인 만큼 복잡하고 다양한 명령어들을 활용한다. 디테일한 명령어를 사용하기 때문에 적은 수의 명령어로 프로그램을 실행할 수 있다. 그래서 메모리 공간을 절약하고자 할때 인기가 많았다. 다만 명령어가 복잡하고 다양하기 때문에 명령어의 크기와 실행되기까지의 시간이 일정하지 않다(규격화되지 않았다). 그래서 명령어 하나를 실행하는 데 여러 클럭 주기가 필요하다. 즉 명령어 파이프라인을 구현하기 쉽지 않다. 현대 CPU에서 명령어 파이프라인은 높은 성능을 위한 핵심 기술이므로 이 단점을 보완하고자 RISC가 등장한다.

#### RISC: Reduced ISC
- 명령어길이와 수행시간을 짧고 규격화하고자 했고, 복잡한 기능을 지원하는 명령어보다 자주 쓰이고 기본적인 명령어를 작고 빠르게 만들고자 했다.
- 되도록 1클럭 내외로 실행되는 명령어를 지향해 고정 길이 명령어를 활용한다. 
- 메모리 접근을 단순화/최소화하고자 메모리에 직접 접근하는 명령어를 load, store 두개로 제한한다. 대신 레지스터를 적극 활용한다. CISC보다 레지스터를 이용한 연산이 더 많고, 사용하는 명령어 갯수는 더 적기 때문에 더 많은 명령으로 프로그램을 작동시킨다.

## 송현

### 중요
명령어 집합 or 명령어 집합 구조(ISA; Instruction Set Architecture) : CPU가 이해할 수 있는 명령어들의 모음 

ISA를 기반으로 설계된 파이프라이닝 하기 쉬운 명령어는 CISC와 RISC 두 가지가 있다.

CISC; Complex Instruction Set Computer : 다양하고 강력한 기능의 명령어 집합을 활용하기 때문에 명령어의 형태와 크기가 다양한 가변 길이 명령어를 활용한다.
 - 장점 : 메모리 공간을 절약할 수 있다
 - 단점 : 복잡하고 다양한 명령어의 크기와 실행되기까지의 시간이 일정하지 않았다. -> 명령어 하나에 여러 클럭 주기가 필요함 -> 규격화되지 않는 명령어가 파이프라이닝을 어렵게 만듦 -> 명령어 파이프라인이 제대로 동작하지 않는 CPU의 아주 치명적인 약점 / 명령어 집합 중 20% 정도가 전체의 명령어의 80%가량을 차지함 (결국 쓰는 명령어만 사용

RISC; Reduced Instruction Set Computer : 단순하고 적은 수의 고정 길이 명령어 집합을 활용한다. 
 - 장점 : 짧고 규격화된 명령어를 활용하기에 명령어 파이프라이닝에 유리함
### 문제
### 답

