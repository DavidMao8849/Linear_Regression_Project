## 📈 주택가격 예측 프로젝트 - 회귀분석 기반 부동산 모델링
**인공지능과 데이터과학(2) PBL 프로젝트 - 능지공인팀**  
> 팀원: 이은우<br/>
> 프로젝트 기간: 2024년 11월 10일 ~ 2024년 12월 1일

---

## 📌 프로젝트 개요
서울시 부동산 실거래 데이터를 기반으로 **"건물의 면적", "층수", "건축년도"** 등의 특성을 이용하여 **건물 가격을 예측**하는 머신러닝 프로젝트입니다.  
기본적인 회귀 분석의 적용부터 데이터 전처리, 모델 학습 및 평가까지 전체 머신러닝 파이프라인을 경험할 수 있습니다.

### ✅ 선정 배경
- **주제**: 머신러닝 수업을 들으며 가장 쉽게 설명할 수 있는 회귀분석의 예로 항상 **부동산 가격 예측**을 예로 들었었다.<br/>
이 쉬운 예시를 토대로 실제 부동산 데이터를 이용해서 회귀 분석을 하게 되면 어떨까 라는 취지로 해당 주제를 선정하였다. 

---

## 🛠️ 사용 기술
- **언어 및 라이브러리**: Python, Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib  
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

## 📷 프로젝트 이미지

<details>
<summary>결과물 보기</summary>
  
## 웹 디자인 및 구조 설계
<img src="https://github.com/user-attachments/assets/52e2e0c8-8761-4208-b8c4-fb95a2c0b07e"/>
<img src="https://github.com/user-attachments/assets/9e5fb3ac-aa15-4221-88a9-43444ad45dda"/>

## 개발 회의[디스코드 화면공유 이용]
<img src="https://github.com/user-attachments/assets/0975be43-ea07-4f8b-975f-aa81ccd5aea2"/>
<img src="https://github.com/user-attachments/assets/84b965d5-d84e-491a-be36-c5d3c0e46f0a"/>
  
## 메인 웹 폼[메인화면]
<img src="https://github.com/user-attachments/assets/cc098d46-e34d-4a05-8b38-3b812447d419"/>
[코드 내용]https://github.com/DavidMao8849/Movie_Recommend_Project/blob/a5375c53a326d5de191bd83fb29e98753ac956a2/MovieMain.aspx#L1-L33

## 리스트 웹 폼[역대 흥행 영화 찾아보기]
<img src="https://github.com/user-attachments/assets/ca78f735-93fd-4fd3-937f-f5c7b223788f"/>
<img src="https://github.com/user-attachments/assets/7744b549-9799-4888-b540-f31efb51ba7e"/><br />
[코드 내용]https://github.com/DavidMao8849/Movie_Recommend_Project/blob/a5375c53a326d5de191bd83fb29e98753ac956a2/MovieList.aspx#L1-L78

## 다시보기 웹 폼[장르별 다시 볼 영화 추천]
![image](https://github.com/user-attachments/assets/d229cf6e-5c5f-4195-975f-48409c9a0ac8)
![image](https://github.com/user-attachments/assets/073f50d8-8782-488b-b9f4-5a4eb299c2d4)<br />
[코드 내용]https://github.com/DavidMao8849/Movie_Recommend_Project/blob/a5375c53a326d5de191bd83fb29e98753ac956a2/MovieReview.aspx#L1-L79

## 제작자 웹 폼[팀 이름 및 팀원 역할 ]
![image](https://github.com/user-attachments/assets/9d0f1a82-a324-4b1f-998e-6e3403c8d82d)<br />
[코드 내용]https://github.com/DavidMao8849/Movie_Recommend_Project/blob/74e04f01554d84551c4143e630d6f095a7f47022/MovieMaker.aspx#L1-L57

</details>

---

## 💡 기대 효과 및 활용 방안
- 부동산 거래 시 빠른 가격 예측 가능
- 투자 및 정책 결정에 참고 가능한 분석 도구
- 가격 형성 요인의 이해에 도움
- 부동산 관련 애플리케이션 개발에 활용 가능

---

## 📎 부록
- 발표 자료: [`발표.pptx`](docs/발표.pptx)
- 결과 보고서: [`결과보고서.pdf`](docs/PBL결과보고서.pdf)

---
