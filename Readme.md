## 📈 주택가격 예측 프로젝트 - 회귀분석 기반 부동산 모델링
**인공지능과 데이터과학(2) PBL 프로젝트 - 능지공인팀[개인]** 
> 프로젝트 기간: 2024년 11월 10일 ~ 2024년 12월 1일

---

## 📌 프로젝트 개요
서울시 부동산 실거래 데이터를 기반으로 **"건물의 면적", "층수", "건축년도"** 등의 특성을 이용하여 **건물 가격을 예측**하는 프로젝트입니다.  
기본적인 회귀 분석의 적용부터 데이터 전처리, 모델 학습 및 평가까지 전체 머신러닝 파이프라인을 경험할 수 있었습니다.

### ✅ 선정 배경
- **주제**: 머신러닝 수업을 들으며 가장 쉽게 설명할 수 있는 회귀분석의 예로 항상 **부동산 가격 예측**을 예로 들었었다.<br/>
이 쉬운 예시를 토대로 실제 부동산 데이터를 이용해서 회귀 분석을 하게 되면 어떨까 라는 취지로 해당 주제를 선정하였다. 

---

## 🛠️ 사용 기술
- **언어 및 라이브러리**: Python, Pandas, NumPy, Scikit-learn, Matplotlib  
- **모델링**: 선형회귀, 랜덤 포레스트 회귀 (RandomForestRegressor)
- **평가 지표**: MSE, MAPE, R² Score
- **하이퍼파라미터 튜닝**: RandomizedSearchCV
- **시각화**: 산점도, 히스토그램, 회귀선 등

## 📂 데이터
- **출처**: 서울 열린데이터 광장 (공공데이터 포털)
- **형태**: CSV (서울시 부동산 실거래가 정보)
- **전처리 작업**<br/>
  └─ 필터링: 개봉동, 오류동, 온수동 데이터만 사용<br/>
  └─ 결측값 제거<br/>
  └─ 파생 변수 생성 (예: 연식 = 현재년도 - 건축년도)<br/>
  └─ 로그 변환 적용<br/>
  └─ 데이터 스케일링(StandardScaler)<br/>
---

## 🔍 회귀 분석 과정
1. **데이터 로딩 및 전처리**
2. **특징 선택 및 파생 변수 생성**
3. **로그 변환 및 스케일링**
4. **학습/테스트 데이터 분리**
5. **모델 학습 (RandomForestRegressor)**
6. **하이퍼파라미터 튜닝**
7. **모델 평가 및 시각화**
8. **사용자 입력값 기반 예측 구현**

---

## 📊 결과 시각화
- **히스토그램**: 예측값 vs 실제값의 분포 비교
- **산점도**: 각 특징별 예측값과 실제값의 관계 시각화
- **회귀선 시각화**: 모델의 추세선을 시각적으로 확인

---

## 🖼 결과 시연 화면

<details>
<summary>결과물 보기</summary>
  
## 데이터 셋 CSV파일
![image](https://github.com/user-attachments/assets/630605ab-9c9f-4fb5-ba4d-b08920dd1a3f)

## 데이터 전처리 작업
https://github.com/DavidMao8849/Linear_Regression_Project/blob/d16b2c17fe00661a7321b0222b29cabc9ac6b1b1/pbl%5B%ED%9A%8C%EA%B7%80%EB%B6%84%EC%84%9D%5D.py#L20-L23
![image](https://github.com/user-attachments/assets/317677b2-94bc-460c-b4f1-367f8737814b)
https://github.com/DavidMao8849/Linear_Regression_Project/blob/d16b2c17fe00661a7321b0222b29cabc9ac6b1b1/pbl%5B%ED%9A%8C%EA%B7%80%EB%B6%84%EC%84%9D%5D.py#L27-L49
![image](https://github.com/user-attachments/assets/0d666a7f-b8f1-43ca-9318-513116ebcc91)
  
## 모델 생성 및 학습 결과
https://github.com/DavidMao8849/Linear_Regression_Project/blob/d16b2c17fe00661a7321b0222b29cabc9ac6b1b1/pbl%5B%ED%9A%8C%EA%B7%80%EB%B6%84%EC%84%9D%5D.py#L67-L122
![image](https://github.com/user-attachments/assets/b3188f29-3fbf-419f-ad45-3061a96e4e35)


## 학습결과 시각화
https://github.com/DavidMao8849/Linear_Regression_Project/blob/d16b2c17fe00661a7321b0222b29cabc9ac6b1b1/pbl%5B%ED%9A%8C%EA%B7%80%EB%B6%84%EC%84%9D%5D.py#L126-L136
![image](https://github.com/user-attachments/assets/8d5f9473-6279-49a5-ad56-2bb039889550)

- ### 선형회귀 그래프<br/>
https://github.com/DavidMao8849/Linear_Regression_Project/blob/d16b2c17fe00661a7321b0222b29cabc9ac6b1b1/pbl%5B%ED%9A%8C%EA%B7%80%EB%B6%84%EC%84%9D%5D.py#L138-L164
![image](https://github.com/user-attachments/assets/307671cb-365e-4fd5-b243-41fa025fb84e)

- ### 산점도로 볼시<br/>
https://github.com/DavidMao8849/Linear_Regression_Project/blob/d16b2c17fe00661a7321b0222b29cabc9ac6b1b1/pbl%5B%ED%9A%8C%EA%B7%80%EB%B6%84%EC%84%9D%5D.py#L166-L192
![image](https://github.com/user-attachments/assets/270ebf4f-28cb-4bee-9543-6179bdd0f348)

## 임의의 데이터로 예측하기
https://github.com/DavidMao8849/Linear_Regression_Project/blob/d16b2c17fe00661a7321b0222b29cabc9ac6b1b1/pbl%5B%ED%9A%8C%EA%B7%80%EB%B6%84%EC%84%9D%5D.py#L194-L208
![image](https://github.com/user-attachments/assets/deae9e65-6abe-43e7-8e33-bfccd92abe8b)
![image](https://github.com/user-attachments/assets/f09966d6-bf33-4af2-87c7-2dedd3a99fbb)

</details>

---

## 🩹 프로젝트에서 겪었던 문제점
**모델의 오차가 너무 높았던 점.**
   - 해당 프로젝트에서 회귀분석 예측치의 오차를 20% 이내로 맞춰야 했음.<br>
    **문제해결(데이터 전처리 부분)**<br/>
       └─ 파생 변수 생성 (예: 연식 = 현재년도 - 건축년도)<br/>
       └─ 로그 변환 적용 (타겟 = 물건 가격)<br/>
    **문제해결(모델 설계/학습 부분)**<br/>
       └─ 데이터 스케일링 이용<br/>
       └─ 하이퍼 파라미터 튜닝 (RandomForest)<br/>

## 💡 기대 효과 및 활용 방안
- 부동산 거래 시 빠른 가격 예측 가능
- 투자 및 정책 결정에 참고 가능한 분석 도구
- 가격 형성 요인의 이해에 도움
- 부동산 관련 애플리케이션 개발에 활용 가능

---

## 📎 부록
- 발표 자료: [`발표.pptx`](docs/인공지능과_데이터과학_능지공인팀_PBL_발표_PPT.pptx)
- 결과 보고서: [`결과보고서.pdf`](docs/PBL_결과보고서_요약본_인공지능과데이터과학(2)-능지공인팀.pdf)

---
