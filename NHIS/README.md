# Project Description

이 레포지토리는 공공데이터포털에서 제공하는 데이터를 활용하여 데이터 분석을 수행하는 프로젝트다.

# Data Source

[공공데이터포털](https://www.data.go.kr/tcs/eds/selectCoreDataListView.do)

# Data Extraction Date

2024.12.23

# Data Files

1. 본 프로젝트에서 활용 가능한 데이터는 다음과 같다.
    - 국민건강정보데이터
        - NHIS_HealthCheckupData_2023.csv
        - NHIS_MedicationPrescriptionInfo_2023_1.csv
        - NHIS_MedicationPrescriptionInfo_2023_2.csv
        - NHIS_MedicationPrescriptionInfo_Appendix_ActiveIngredientCodeChangeHistory.csv
	    - NHIS_MedicalTreatmentInfo_2023.csv

2. 데이터 분석 작업은 위 파일 중 하나 또는 그 이상을 선택하여 진행한다.

# Dependencies

본 프로젝트는 conda 환경을 통해 패키지를 관리한다. 필요한 의존성은 environment.yml 파일로 관리한다:

environment.yml의 예

```yml
name: my_environment
channels:
	•	defaults
	•	conda-forge
dependencies:
	•	numpy=1.26.4
	•	pandas=2.1.4
	•	matplotlib=3.8.0
	•	seaborn=0.12.2
	•	scipy==1.11.3
```

추가한 의존성을 가상 환경에 설치할 땐 다음의 명령어를 사용한다.

`conda env update –name [conda virtual environment name] –file environment.yml --prune`

# Usage
1.	이 레포지토리를 클론한다.
2.	conda 환경을 생성/업데이트한다.
3.	데이터에 대한 매뉴얼을 읽으면서 데이터 자체를 이해한다.
4.  Jupyter Notebook 혹은 Python 스크립트로 분석을 진행한다.
