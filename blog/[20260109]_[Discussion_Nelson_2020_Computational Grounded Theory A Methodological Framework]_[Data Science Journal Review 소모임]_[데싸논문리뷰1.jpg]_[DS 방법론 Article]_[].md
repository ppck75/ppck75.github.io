# 데이터사이언스 논문 리뷰 소모임_20261009
## Computational Grounded Theory: A Methodological Framework_Nelson (2020)
### 경희대학교 전혁식 교수님


**Computational Science 또는 Data Science 관련 논문을 리뷰하는 소모임에서 토론한 내용과 저의 생각을 자유롭게 정리한 글입니다.**

Laura K. Nelson의 Computational Grounded Theory:A Methodological Framework(2020) Article을 리뷰하였습니다.

**논문 정리 게시글 바로가기 -> [Computational Grounded Theory:A Methodological Framework(2020) 논문정리](https://ppck75.github.io/weniv_blog/?post=%5B20260107%5D_%5BNelson_2020_Computational+Grounded+Theory+A+Methodological+Framework%5D_%5BData+Science+Journal+Review%5D_%5B%EB%8D%B0%EC%8B%B8%EB%85%BC%EB%AC%B8%EB%A6%AC%EB%B7%B01.jpg%5D_%5BDS+%EB%B0%A9%EB%B2%95%EB%A1%A0+Article%5D_%5B%5D.md)

---

## 1. 논문 개요 및 문제의식

이 논문은 **Computational Grounded Theory(CGT)**라는 **방법론적 프레임워크(3단계)**를 제안하는 논문이다. 저자는 기존 근거이론(grounded theory)의 이론 생성 논리를 유지하면서, 대규모 텍스트 자료를 다루는 현대 사회학 연구에서 계산 기법을 체계적으로 결합하는 절차를 제시한다.

---

### 2. 근거이론(Grounded Theory)

근거이론은 이론이란 잘 관찰된 근거, 즉 데이터로부터 출발해야 한다는 인식에 기반한다. 기존 양적 연구와 달리 선행연구에 기반한 가설 검증이 아니라, **현장에 존재하는 날 것의 자료(substantive data)**를 토대로 새로운 이론을 생성하는 것을 목표로 한다. 즉, 근거이론은 **현장 기반의 새로운 이론 발견**을 핵심으로 한다.

---

## 3. Computational Grounded Theory의 3단계 구조

### Step 1. Pattern Detection

첫 번째 단계는 **계산 기반의 귀납적 탐색 단계**이다.
이 단계는 계산 기법을 활용해 복잡한 텍스트를 해석 가능한 단어 집합으로 축소한다.

### Step 2. Pattern Refinement

두 번째 단계는 **질적 해석과 deep reading**을 통해 패턴을 정교화하는 단계다.
이 단계에서 연구자는 범주를 명명하고, 경계를 설정하며, 사회학적 의미를 부여한다.

### Step 3. Pattern Confirmation

세 번째 단계는 앞선 두 단계에서 도출된 패턴이 **우연이나 특정 알고리즘의 산물이 아님을 검증**하는 단계다.

---

## 4. Computer-assisted Text Analysis의 세 가지 범주

### ① Lexical-based techniques
- 단어·구 빈도, word scores, 공기어 네트워크
- 분석 단위: 단어 / 구
- 의미 해석은 연구자의 몫

**즉,**  
*무슨 단어가, 얼마나, 어디서 등장하는가*

### ② Machine-learning–based text classification
- 지도학습 / 비지도학습(토픽 모델링)
- 문서는 여러 토픽의 혼합물이라는 가정

**즉,**  
*이 텍스트는 어떤 범주(들)에 속하는가*

### ③ Natural Language Processing (NLP)
- 품사, 문맥, 문장 구조 반영
- 의미에 더 가까운 근사 가능

**즉,**  
*이 단어는 어떤 문맥과 역할로 쓰였는가*

---

## 5. 토픽 모델링과 파라미터 문제

토픽 모델링은 효율적이고 직관적인 도구이지만, 토픽 수(k), 전처리 방식 등 연구자의 선택에 매우 민감하다. 저자는 단일 모델을 최적이라고 주장하는 태도를 경계하며, 여러 모델을 비교해야 함을 강조한다.

> “To determine which model was best for my corpus, I ran four topic models, with 20, 30, 40, and 50 topics, respectively…”  
> (Nelson, 2020)

이 사례는 토픽 수가 너무 적을 경우 이질적 주제가 결합되고, 너무 많을 경우 동일 주제가 과도하게 분할될 수 있음을 보여준다.

---

## 6. Step 1의 목적과 parse의 의미

Step 1의 계산적 패턴 탐지는 두 가지 목적을 가진다.

> “Taken together, this first, computational pattern detection step serves two purposes…”  
> (Nelson, 2020)
또한 계산 기법은 텍스트를 빠르고 신뢰롭게 처리하여 재현성을 확보한다.

> “Second, as these techniques parse text quickly and reliably, they are both more efficient than a researcher reading through the text and they are completely reproducible.”  
> (Nelson, 2020)

여기서 *parse*란 텍스트를 일정한 규칙에 따라 분해해 계산 가능한 구조로 변환하는 것을 의미한다.

---

## 7. Step 2: Deep Reading

Deep reading은 계산 결과를 바탕으로 연구자가 텍스트를 다시 읽으며 해석을 수행하는 단계다.

> “This makes the process more efficient, but it also ensures the researcher will not skip over important passages because of fatigue or bias.”  
> (Nelson, 2020)

---

## 8. Step 3: Pattern Confirmation

Step 3에서는 지도학습, NLP, 사전 기반 방법 등을 통해 패턴을 검증한다.

> “Supervised machine learning is a common method used to confirm and calculate themes or patterns in text.”  
> (Nelson, 2020)

저자는 자신의 연구에서 NLP 기법과 사전 기반 방법을 사용했다고 밝힌다.

> “In my research, I used various natural language processing techniques as well as one dictionary method to confirm and provide more evidence to support the patterns identified in the first two steps.”  
> (Nelson, 2020)

---

## 9. 결론

이 논문은 계산 기법을 이론 생성의 대체물이 아니라 **이론 생성을 돕는 구조적 장치**로 재위치시킨다는 점에서 중요한 방법론적 기여를 한다. CGT는 계산과 해석, 검증을 단계적으로 결합해 **효율성·신뢰성·재현성**을 동시에 확보하려는 시도로 이해할 수 있다.

---

## 10. 토론 질문
- STM은 R에서 제공한다. 파이썬에서는 이를 구현 할 수 있나?

    Aricle에서 제시한 연구자의 깃허브에서 사용한 코드를 확인해보았는데, 토픽 모델링 부분 등은 R로 분석했고, 스텝3 부분 등은 파이썬으로 분석했다. 교수님께서도 이런 식으로 자주 혼합하여 사용하시는지?

> STM은 R에서 제공하는 패키지! 교수님께서는 **BERTopic**을 주로 사용하신다.
> BERTopic(버트토픽)은 BERT 기반 문장 임베딩 + 군집화 + 단어 중요도 추출을 결합한 의미 중심 토픽 모델링 방법이다. 이는 단어 빈도가 아니라 문서의 의미로 토픽을 만드는 모델이다.

    기존 토픽 모델링(LDA)는 단어 동시 등장 확률, 단어 빈도 패턴을 중심으로 토픽을 만든다. 이는, 짧은 텍스트, 은유적 표현, 담론적 의미에 약하다. 

    하지만, BERTopic은 문서를 문장 벡터(의미 벡터)로 바꾼 뒤, 의미가 비슷한 문서들을 묶어 토픽을 형성한다 

**BERTopic의 전체 구조**

① 문서 → 문장 임베딩(임베딩이란 텍스트를 컴퓨터가 계산할 수 있는 숫자 벡터로 바꿔서 의미가 있는 것끼리 가깝게 놓게 만드는 표현 방식이다)

- BERT 계열 모델로 각 문서를 벡터화

- “단어”가 아니라 문서의 의미를 수치로 표현

    단어 임베딩은 단어하나가 벡터 하나. 왕과 영왕은 비슷한 위치, 사과는 과일과 비슷한 위치! 문장 임베딩은 문장, 짧은 글 하나가 벡터 하나. 문장 전체의 뜻(문맥)을 요약한 좌표이다. 즉, 단어가 완전히 같지는 않아도 문장의 의미가 비슷해서 벡터가 가까워질 수 있다. 

    즉, BERTopic은 각 문서를 문장 임베딩으로 바꾸고, 임베딩이 서로 가까운 문서들끼리 묶어서 군집화한다. 그 묶음의 대표 단어를 뽑아서 '토픽'을 만든다. 즉, 단어 빈도가 아니라 문서 의미의 거리로 토픽을 만드는 모델링이다. 

② 차원 축소 (UMAP)

- 고차원 벡터를 저차원으로 압축

- 의미 구조는 유지하면서 군집화가 쉬워짐

③ 군집화 (HDBSCAN)

- 군집 개수를 자동 결정

- 애매한 문서는 아웃라이어로 제외 가능 → 사회과학 데이터에 매우 중요

④ 토픽 단어 추출 (c-TF-IDF)

- 각 군집(토픽)에서

- 그 토픽에만 특징적인 단어를 계산 → 토픽의 “의미적 이름표



- 토픽 모델링에서 파라미터 결정에 도움이 되는 다른 방법이 없을까?

    논문에서는 가이드라인이 따로 없다는 것으로 이해했다. 그런데, 비지도학습 중 K-means 클러스터링의 경우 elbow method나 실루엣 스코어로 파라미터 설정에 도움을 받을 수 있고, 왜 이런 군집 수를 설정했는지 제시를 할 수 있다. 그래서 이러한 방식이 토픽 모델링에는 없는지 궁금하다. 

- 토픽 모델링에서 토픽 수를 어떻게 설정하느냐에 따라 모델링의 결과가 달라진다. 이것을 머신러닝의 과대적합, 과소적합의 논리로 이해하면 될까?

    k가 너무 작을 때는 서로 다른 주제를 하나의 토픽 안에 욱여넣을 우려가 있다. 즉 모델은 의미 구분을 포기하고 통계적 타협을 한다. 
    k가 너무 클 때에는 과잉 분할이 일어난다. 즉, 모델은 차이를 만들어내기 위해 의미 없는 분리를 한다. 

- 14페이지의 토픽 모델링 그림에 대한 질문
    왜 렉시컬 셀렉션과 토픽 모델링이 이 그림에서 왼쪽으로 빠질까? 잘 와닿지 않는다. 
---

## 11. 그 밖에 개념 정리 
1. 근거이론
    근거이론은 일관성 있는 이론을 위해 구조를 찾아야 하며, 모든 구조는 잘 관찰된 근거, 즉, 데이터로부터 시작된다고 본다. 여기서 양적연구와 근거이론이 다른 점은 선행연구에 기반하지 않은 실체적 속성의 자료에 근거하거나, 토대를 두고 이론개발을 하려한다는 점이다. 즉, 근거 이론은 현장 있는 날 것의 자료에 기반해 새로운 이론을 창출한다. (현장에 기반한 새로운 이론 발견) 

2. Corpus란?
    언어 처리 분야에서 컴퓨터로 분석할 수 있도록 모아놓은 대량의 언어 데이터 집합을 뜻합니다.

3. 파싱이란?
    텍스트를 일정한 규칙에 따라 잘게 분해하고, 각 요소를 처리 가능한 단위로 변환하는 것. 즉, 텍스트를 분석 가능하고 계산가능한 구조로 바꾸는 것이 파싱이다

4. Deep reading
    Deep reading은 계산 기법이 제시한 패턴을 바탕으로,
    연구자가 텍스트를 다시 ‘맥락·의미·사회적 함의’ 수준에서 면밀히 해석하는 질적 분석 단계다.
    여기서 연구자는:
    •	범주 이름을 붙이고
    •	경계를 정하고
    •	조건을 설명하고
    •	사회학적 의미를 부여함

    전통적 질적 독서: 처음부터 끝까지 읽음, 연구자 직관 중심, 소규모 데이터,재현 어려움
    CGT의 Deep reading: 계산 결과가 읽을 대상을 선별, 계산으로 탐색 범위 축소, 대규모 데이터 일부, 어떤 텍스트를 읽었는지 명시 가능
  


## References

Nelson, L. K. (2020). *Computational grounded theory: A methodological framework*.  
*Sociological Methods & Research, 49*(1), 3–42.  
https://doi.org/10.1177/0049124117729703

