# Emotify : 텍스트에 감정을 더하다

## 1️⃣ 프로젝트 개요

때로는 감정을 담아 글을 적는 것은 어려운 일이 됩니다.📝 자신의 감정을 정확히 표현하지 못해 답답함😮‍💨을 느끼는 사람들을 위해, 감정을 풍부하게 만드는 **텍스트 생성기**를 만들었습니다.

본 프로젝트 는 사용자가 작성한 **일기를 분석**하여 감정에 맞는 **이모지를 삽입**🤩하는 서비스입니다. 이를 통해 사용자가 자신의 감정을 더 직관적으로 표현하고, 글의 분위기를 풍부하게 만들 수 있도록 돕습니다.

또한, **부정적 감정**이나 **위험 신호🚨를 감지**하여 경고하는 **레드플래그 시스템** 🚩을 통해 감정 관리의 중요성을 강조합니다.

## 2️⃣ 플로우 차트
<img width="800" alt="스크린샷 2024-11-26 오후 6 13 09" src="https://github.com/user-attachments/assets/c8b200ee-0bbf-4696-89c1-d16e9f6caef6">

## 3️⃣ 모델링 과정
> 신조어 치환
- 신조어 사전 생성# Emotify : 텍스트에 감정을 더하다

## 1️⃣ 프로젝트 개요

때로는 감정을 담아 글을 적는 것은 어려운 일이 됩니다.📝 자신의 감정을 정확히 표현하지 못해 답답함😮‍💨을 느끼는 사람들을 위해, 감정을 풍부하게 만드는 **텍스트 생성기**를 만들었습니다.

본 프로젝트 는 사용자가 작성한 **일기를 분석**하여 감정에 맞는 **이모지를 삽입**🤩하는 서비스입니다. 이를 통해 사용자가 자신의 감정을 더 직관적으로 표현하고, 글의 분위기를 풍부하게 만들 수 있도록 돕습니다.

또한, **부정적 감정**이나 **위험 신호🚨를 감지**하여 경고하는 **레드플래그 시스템** 🚩을 통해 감정 관리의 중요성을 강조합니다.

## 2️⃣ 플로우 차트
<img width="800" alt="스크린샷 2024-11-26 오후 6 13 09" src="https://github.com/user-attachments/assets/c8b200ee-0bbf-4696-89c1-d16e9f6caef6">

## 3️⃣ 모델링 과정
> 신조어 치환
- 신조어 사전 생성
![스크린샷 2024-11-26 182320](https://github.com/user-attachments/assets/2cacbdc3-d2cb-4f84-9da0-151db7e81252)

> 감정 분석
- KcELECTRA 모델 사용
- 데이터 전처리 : label - ʻ*발화*’, ʻ*감정*’
    - 7개의 감정으로 분류 (행복, 중립, 슬픔, 공포, 혐오, 분노, 놀람)
    
> 문장 유사도 분석 + 레드플래그
<img width="300" alt="스크린샷 2024-11-26 오후 6 13 09" src="https://github.com/user-attachments/assets/fa067210-0c45-412e-8afd-cf28ae83cf9e">

- 데이터 전처리 : label - *ʻtext*’, ’*keyword*’
- 실제 정신 상담 데이터를 **SBERT**로 문장 임베딩 후 키워드 별 평균 벡터 구해 코사인 유사도 측정
- 고위험, 중위험 감정으로 분류해 레드플래그 🚩 감지

## 4️⃣ 시연 화면
> 이모지 삽입
<img width="500" alt="스크린샷 2024-11-26 오후 6 16 42" src="https://github.com/user-attachments/assets/f12bcda7-4a33-4e84-831b-ebe559f910f1">

> 레드플래그 감지
<img width="500" alt="스크린샷 2024-11-26 오후 6 15 52" src="https://github.com/user-attachments/assets/d85e1e95-31d1-444b-ae14-b48f659a05fc">

## 5️⃣ 팀원



|<img src="https://avatars.githubusercontent.com/" width="100"/>|<img src="https://avatars.githubusercontent.com/" width="100"/>|<img src="https://avatars.githubusercontent.com/" width="100"/>|<img src="https://avatars.githubusercontent.com/u/111039206?v=4" width="100"/>|
|:---:|:---:|:---:|:---:|
|[김동혁](https://github.com/)|[김혜란](https://github.com/)|[이동진](https://github.com/)|[장영주](https://github.com/youngju6143)|


