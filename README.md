# INSIGHT 15th
26년도 상반기 14기, 15기 활동 레포입니다!

## 심화세션 목표
- 앙상블 기법을 통해 기존 머신러닝 모델의 성능을 향상할 수 있습니다.
- 퍼셉트론과 딥러닝의 기초를 다지고, Colab, GitHub, Hugging Face 사용에 익숙해집니다.
- 이미지, 시퀀스, 시계열 등 다양한 형태의 데이터를 딥러닝 모델로 처리할 수 있습니다.
- 트랜스포머, 언어 모델 및 생성 모델의 원리를 이해하고 적용할 수 있습니다.
- 추천 시스템을 구축하고, 모델 최적화 기법과 최신 AI 트렌드를 파악할 수 있습니다.


## 진행 기간 및 내용
| 회차 | 세션일자 - 과제 마감일 | 내용 |
| --- | --- | --- |
| 1 | 4/30 - 5/3 | 앙상블 & Colab |
| 2 | 5/4 - 5/6 | 퍼셉트론 & 딥러닝 기초 & Hugging Face |
| 3 | 5/7 - 5/10 | 딥러닝 1: FOCUS ON IMAGE & SEQUENCE |
| 4 | 5/11 - 5/13 | 딥러닝 2: FOCUS ON TRANSFORMER |
| 5 | 5/14 - 5/17 | 언어 모델 |
| 6 | 5/18 - 5/20 | 생성 모델 & AI 최적화 |
| 7 | 5/21 - 5/27 | 추천 시스템 |
| 8 | 5/28 - 5/31 | 시계열 |
| 9 | 6/1 - | AI 트렌드 |

## 진행 방식
- 매 회차별로 "사전 학습", "과제" 두 가지의 과제가 있습니다.
- 사전 학습의 마감일은 해당 세션의 진행일 전날입니다.
- 과제 마감일은 다음 세션의 진행일 전날입니다.

>예시
3/5 Pandas 세션일 기준, 3/8 자정까지 제출해야 하는 과제는 
**"Pandas 과제"** 와 **"EDA 사전 학습"** 두 가지 입니다.

## 제출 방식 상세
### 한 번만 하면 되는 과정
  - 해당 insight 레포지토리(원격)를 본인의 컴퓨터(로컬)로 clone합니다.
    ```bash
    git clone https://github.com/Insight-Sogang-Univ/insight-15th.git
    ```

### 과제 제출마다 거쳐야 하는 과정
  - 본인의 브랜치로 전환해 과제를 진행합니다.
    ```bash
    # 0. 과제 시작 전 본인 브랜치 위치 확인하기
    git status
    git branch -a

    # On branch gildong(내 브랜치 이름) 뜨면 성공!

    # 1. 메인브랜치에서 템플릿 로드
    git pull origin main
    # 으로 템플릿 가져오기 + 본인 폴더 안에 템플릿 복붙하기

    # + 중간중간 Ctrl + S로 과제 저장하기!

    # 2. 제출할 파일들을 장바구니에 '하나씩' 담기! ( git add . 지양 )
    git add "basic/gildong/session00/판다스_과제.ipynb"
    git add "basic/gildong/session00/EDA_예습과제.ipynb"

    # 3. 포장하기!
    git commit -m "[session00] #00 홍길동 판다스 과제, EDA 사전과제 제출합니다."

    # 4. 깃허브로 보내기!
    ## ☆ 현재 브랜치의 첫번째 커밋일 때! ☆
    git push -u origin gildong
    ## 그 이후에는 이렇게!
    git push

    # 5. 깃허브 웹에서 [develop <- 내 이름 브랜치(ex. gildong)] 설정하고 pull request 등록
    ## PR 창에서 왼쪽(base)을 main이 아닌 develop으로 바꿔주세요!! 꼭!
    ```

## 폴더 구조
[main 브랜치]
```
insight-15th
├── README.md
├── .gitignore
├── .github
├── advanced/template/...    // 심화 세션 템플릿
└── basic/template/...       // 교육 세션 템플릿

```

[develop 브랜치]
```
insight-15th
├── README.md
├── .gitignore
├── .github
├── basic                      // 교육 세션 과제&실습 제출 아카이빙 & 템플릿 폴더
│   ├── gildong                // 학회원 1의 과제 제출 아카이빙 폴더
│   │   └── session00
│   │       └── example.ipynb  // OT 과제 제출 파일
│   │   └── session01
│   │       └── example.ipynb  // 과제 제출 파일
│   │       └── example_사전과제.ipynb // 세션 전 사전 학습 내용 공부 정리 파일
│   │   └── session02
│   │       └── example.ipynb  // 과제 제출 파일
│   │       └── example_사전과제.ipynb // 세션 전 사전 학습 내용 공부 정리 파일
│   │  ... 
│   ├── jiwon                  // 학회원 2의 과제 제출 아카이빙 폴더, gildong 폴더 구조와 동일
│       └── session00/...
│       └── session01/...
│      ...
│   ...
│   ├── template               // 교육 세션 템플릿 모음
│   │   └── session00
│   │       └──  example.ipynb // OT 과제 제출 파일
│   │   └── session01
│   │       └── example.ipynb  // 과제 제출 파일
│   │       └── example_사전과제.ipynb // 세션 전 사전 학습 내용 공부 정리 파일
│   │   └── session02
│   │       └── example.ipynb  // 과제 제출 파일
│   │       └── example_사전과제.ipynb // 세션 전 사전 학습 내용 공부 정리 파일
│      ...
├── advanced                   // 심화 세션 과제&실습 제출 아카이빙 & 템플릿 폴더 (교육세션과 구조 동일)
│   ├── gildong/...
│   ├── jiwon/...
    ...
│   └── template/...           // 심화 세션 템플릿 모음
```

[개인별 브랜치]
```
insight-15th
├── README.md
├── .gitignore
├── .github
├── basic                      // 교육 세션 과제&실습 제출 아카이빙 & 템플릿 폴더
│   ├── gildong
│   │   └── session00
│   │       └── example.ipynb  // OT 과제 제출 파일
│   │   └── session01
│   │       └── example.ipynb  // 과제 제출 파일
│   │       └── example_사전과제.ipynb // 세션 전 사전 학습 내용 공부 정리 파일
│   │   └── session02
│   │       └── example.ipynb  // 과제 제출 파일
│   │       └── example_사전과제.ipynb // 세션 전 사전 학습 내용 공부 정리 파일
│   │  ... 
├───┴── template/...           // 교육 세션 템플릿 모음
├── advanced                   // 심화 세션 과제&실습 제출 아카이빙 & 템플릿 폴더
│   ├── gildong
│   │   └── session01
│   │       └── example.ipynb  // 과제 제출 파일
│   │       └── example_사전과제.ipynb // 세션 전 사전 학습 내용 공부 정리 파일
│   │   └── session02
│   │       └── example.ipynb  // 과제 제출 파일
│   │       └── example_사전과제.ipynb // 세션 전 사전 학습 내용 공부 정리 파일
│   │  ... 
└───┴── template/...           // 심화 세션 템플릿 모음
```



## 제출 양식
**`pull request`** 를 보낼 때 아래의 양식과 같이 보내주세요!
```
pr 제목 : [session세션번호] #이슈번호 이름 —과제, —사전과제 제출합니다.
(단일 커밋을 보냈을 경우, 커밋 메세지가 pr 제목으로 자동 설정 되기도 합니다.)

내용 : 해당 과제를 하면서 어려웠던 점이나 새로 알게 된 점 간단히 정리
```

ex)

## [session01] 최지원 Pandas 과제 제출합니다.


### 🔍 어려웠던 점 및 새로 알게 된 점 간단히 정리
series는 꼼꼼하게 안 써본 부분이었는데 더 명확히 짚고 갈 수 있었습니다.
loc, iloc은 항상 헷갈렸었는데, loc은 파이썬 인덱스, iloc은 정수 인덱스를 사용한다는 차이점을 이해하게 되었습니다.
groupby도 series와 df 두 가지 형태로 반환하는 방법을 알게 되었습니다.


### 🔍 질문 및 하고 싶은 말
로컬에서 push할때도 base를 따로 지정해주는 과정이 있는 것인지 궁금합니다.


### ✅ PR Checklist
PR이 다음 요구 사항을 충족하는지 확인하세요.
- [x] 본인 세션별 브랜치 → develop 브랜치 로 PR 합니다.


## 기타
- 사전 과제 필수 키워드 (해당 세션의 노션 페이지 및 issue에서 확인 가능)에 대해서는 정리/리뷰 하셔야 합니다.
- 사전 학습 정리는 자유 분량입니다.