# Apache Airflow 기반의 데이터 파이프라인

이 저장소에는 매닝 출판사의 [Apache Airflow 기반의 데이터 파이프라인](https://www.manning.com/books/data-pipelines-with-apache-airflow) 한국어판 도서의 예제 소스코드를 포함하고 있습니다.
<p align="center">
<img width="529" alt="cover" src="https://user-images.githubusercontent.com/8121792/149867441-c538fd39-fb84-4f60-b3e7-52f2611ae81e.png">
</p>

### 저장소 구성

이 저장소의 구성은 다음과 같습니다.

```
├── chapter01                # 1장의 예제 소스코드.
├── chapter02                # 2장의 예제 소스코드.
├── ...
├── .pre-commit-config.yaml  # CI를 위한 pre-commit(git commit 수행 전에 자동으로 특정 작업을 수행) 설정 파일.
├── CHANGELOG.md             # 코드 업데이트 변경 사항.
├── LICENSE                  # 코드 라이센스.
├── README.md                # 현재 보고 있는 readme 파일.
└── requirements.txt         # CI 요구사항.
```

*chapterXX* 경로에는 각 장에 대한 예제 코드를 포함하고 있습니다.

각 장은 일반적으로 다음과 같이 구성되어 있습니다.

```
├── dags                  # Airflow DAG 예제 (+ 포함 코드).
├── docker-compose.yml    # 해당 장의 컨테이너 실행을 위해 사용되는 도커 컴포즈 파일.
└── readme.md             # 필요 시, 해당 장의 세부 사항을 위한 readme 파일.
```
### 사용방법

해당 장의 예제를 실행하기 위한 자세한 내용은 각 장의 readme에서 확인할 수 있습니다. 대부분의 코드 예제는 각 장에 제공된 docker-compose.yml 파일과 함께 도커 컴포즈를 사용하여 실행할 수 있습니다. 이 도커 컴포즈 파일은 필요한 리소스를 가동하고 도커로 구성된 이 파일은 Airflow 인스턴스 실행을 시작합니다. 모든 것이 실행되면 독자의 PC 브라우저를 사용하여 Airflow 예제를 실행할 수 있습니다.

이후 일부 장(예: 11장 및 13장)은 설정이 좀 더 필요합니다. 이에 대한 자세한 내용은 해당 장의 readme 문서 및 책의 본문에 설명되어 있습니다.
