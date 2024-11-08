# Perspecive_NewsRec "뉴스에 반하다"

개별 주제 (이슈) 에 대한 다양한 관점의 뉴스를 추천하는 알고리즘 서비스


# 프로젝트 개요

## 문제 인식 : 인지 편향과 확증 편향의 문제
  - 사용자 맞춤 추천 시스템 서비스가 지나치게 제공될 경우 "필터 버블(Filter Bubble)" 현상이 야기됨
    - 필터 버블로 인해 사용자의 기호와 관심사와만 일치하는 정보만 더 접하게 됨
  - 사람은 자신의 신념을 확인하려는 경향이 있음
    - 그러나 자신이 이미 알던 것과 다른 내용은 무시하거나 찾으려 하지 않음
    - 필터 버블로 인해 사용자의 인지 편향이 가속되거나 재생산됨
    - 이러한 인지 편향, 그 중에서도 "자신의 의견과 일치하는 정보는 더 믿고 더 찾아보려는" (신념을 확인하려는) 인지 편향을 "확증 편향" 이라 함
  - 확증 편향이 심화됨으로 인해 발생하는 문제
    - 다른 사람의 의견이나 입장을 덜 고려할 확률이 높아지고 이는 비합리적이고 비효율적인 의사 결정으로 연결됨
    - 나아가 사회 계층 양극화를 비롯한 각종 사회 문제가 야기됨
  - 확증 편향에 대한 관련 연구와 문제 제기의 필요성
    - 한국 사회 및 성격 심리학회에서 "2024년 한국사회가 경계해야 할 심리현상은 '확증 편향'" 으로 선정됨
    - [관련](https://www.yna.co.kr/view/AKR20240103107900530)[기사](https://www.joongang.co.kr/article/25241190#home) 및 [연](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8685219/)[구](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE11312388) 
    - 위의 연구 및 기사들에 따랐을 때, 현재 대부분의 사용자 맞춤 추천 시스템 (알고리즘) 은 확증 편향을 크게 심화시키는 주요 요인으로 꼽힘
  - 확증 편향을 완벽히 없앨 수는 없으나 "완화" 할 수는 있음
    - 편향 완화 (감소) 교육을 받은 피교육자는 한 번의 교육만으로도 인지 편향이 크게 줄었다는 [연구결과](https://www.hec.edu/en/yes-you-can-be-trained-make-better-decisions)가 존재함
    - "확증 편향으로 인한 의도적 합리화에 빠지게 되더라도 동일한 반대 관점에 지속적으로 노출되면 결국 '티핑 포인트(전환점)'에 이르러 신념이 바뀔 수 있다".는 [연구결과](https://edisciplinas.usp.br/pluginfile.php/4912780/mod_resource/content/1/BACKFIRE_TIPPING_POINT_redlawsk2010.pdf)가 존재함
     

## 프로젝트 목표
- 이슈성 정보를 다루는 뉴스에서 기존 관점 다른 관점을 제공해 주어 확증 편향을 완화함
- 비판적인 사고력과 자기 객관화 능력 및 정보 분별력 등의 능력 신장에 도움을 주는 프로그램 구축을 목표로 함

### 왜 "뉴스"인가?
- 공익을 위해 객관성과 균형 잡힌 보도를 추구하는 경우가 다수임
  - 사용자 개개인의 흥미나 취향에 무조건적으로 맞추지 않는 것이 뉴스임
  - 유튜브 알고리즘, 상품 추천 광고 알고리즘 등은 사용자의 기호에 따른 참여를 극대화하기 때문에, 플랫폼 운영 목표와 이 프로젝트의 목표가 상충한다고 판단함
- 같은 이슈에 대해서도 언론사나 기자에 따라 여러 의견이 "정리"되어 있는 매체임
  - 사실에 대한 서술 및 사실 기반의 "의견"을 일목요연하게 정리한 기사가 많음
  - 다른 사람들의 의견과 나의 의견을 비교하며 내가 편향되지 않았는지 생각하는 계기가 될 수 있음

### 왜 "포탈 뉴스" 인가?
- 동영상이나 TV에 비해 텍스트는 속도 조절, 검색, 주요 내용 파악이 용이하여 정보 습득 효율성이 높음
  - 키워드 최적화 기술을 통해 쉽게 검색됨됨
  - 검색 엔진에 최적화되어 제공되며, 검색 엔진 결과 페이지에서 높은 우선순위를 갖게 됨
  - 제목, 부제목, 글머리 기호 등을 사용하여 가독성과 접근성이 향상되어 사용자가 자료를 빠르게 훑고 필요한 정보를 찾을 수 있음
- 텍스트 기반이기 때문에 쉽게 저장하고 공유할 수 있음
- 단어와 문장을 기반으로 사용자의 경험과 의견에 공감하는 내러티브를 만들어 강한 감정적 반응을 유도할 수 있음
  - 사용자가 상상력을 발휘하여 시나리오를 시각화하고 상황에 공감하는 능력을 기르는 데도 도움이 됨
- 참고 자료
  - [방송기자가 말하는 '신문 읽어야 하는 이유'](https://dadoc.or.kr/805). 한국언론진흥재단 <미디어리터러시> 블로그. 2013.
  - [Video Content vs. Written Content: Which One Reigns Supreme?](https://www.linkedin.com/pulse/video-content-vs-written-which-one-reignssupreme-mirald-scale-qxtkf). Mirald Scale Content. 2023




## Flow Chart

![image](https://github.com/deepshadow25/Perspecive_NewsRec/assets/115054681/cdbd1b90-e80d-4e3c-b209-893faa7007a5)


## 사용법 설명

Google Chrome Extension 기반 작동
1. 확장 프로그램 설치
2. 설치한 프로그램을 작동시키고 뉴스 웹페이지에 접속
3. 프로그램이 작동되며 기사 주요 부분에 하이라이트 처리가 나타남
4. 하이라이트 처리된 문장에 커서를 가져다 대면 다른 관점의 추천 뉴스를 미리볼 수 있음
5. 하이라이트 처리된 문장에 커서를 클릭하면 미리보기한 뉴스 웹페이지로 이동
6. 이후 프로그램이 작동되는 동안 과정 3-5가 반복됨

# 데이터 설명

- 네이버 뉴스 크롤링 수집 코드
  - 매일 22시마다 기사 자동 수집
  - [우리나라 뉴스 포탈 점유율 중 92%인 네이버](https://www.kpf.or.kr/front/research/selfDetail.do?seq=595996)를 선정
- 사용하는 요소 : 기사제목, 기사링크, 기사본문
  - 수집한 기사 본문 바탕으로 요약문장 뽑아내기
  - 언론사 정보도 수집하지만, 전처리에만 이용하고 삭제함

## 왜 "기사 본문" 전체를 수집하는가?
- 기사 본문을 전부 읽어 맥락을 파악하는 것과 기사 요약본, 제목만 읽고 맥락을 파악하는 점은 다름
- 기사 본문을 전부 수집한 뒤 요약하여, 요약과 유사한 문장에 형광펜과 같은 하이라이트 처리를 하기 위해 기사 본문을 수집


[상세 데이터 설명](https://github.com/deepshadow25/Perspecive_NewsRec/blob/main/Dataset/dataset.md)



# 모델 설명

## 임베딩 및 문서 요약 모델

- 수집한 뉴스 기사의 본문을 임베딩
  - [KPFBERT](https://github.com/KPFBERT/kpfbert) 모델을 이용하여 기사를 [요약](https://github.com/KPFBERT/kpfbertsum) 및 임베딩 처리
  - 또한 클러스터링을 위해 기사를 단락별로 나누고, 이를 임베딩 처리하였음
  - 최종적으로 DB에는 기사제목, 기사링크, 기사본문, 본문 요약과 요약임베딩, 본문 단락별 나눔 및 단락별 임베딩이 들어가게 됨됨


## 뉴스 추천 모델

### 뉴스 추천 모델의 작동 방식

웹 브라우저 점유율이 가장 높은 구글 크름의 확장 프로그램 환경에서 구현
프로그램을 구동하면 현재 읽는 기사의 링크가 서버에 전송되는 것으로 작동을 시작함

### 뉴스 추천 모델의 알고리즘
    1. 현재 읽고 있는 기사의 링크를 서버에 전송
    2. 현재 읽고 있는 기사 본문을 추출 및 요약
      3. 요약한 본문을 DB 내 수집된 요약, 단락별 임베딩과 유사도 비교
      4. 비교한 유사도를 토대로 상위 100건의 유사 기사 (같은 주제를 다루는 뉴스) 추려내기
      5. 4에서 추려낸 뉴스들에 대하여 클러스터링을 통해 관점 나누기. 중심 토픽과의 거리 비교
      6. 5에서 거리가 가장 먼 토픽을 기준으로 3개의 뉴스 링크 추출
    7. 현재 읽고 있는 기사의 링크와 본문, 6의 결과를 종합하여 뉴스 하이라이트, 링크 및 미리보기 표시

### 이용한 모델

유사도 분석 : [KPFSBERT](https://github.com/KPFBERT/kpfSBERT)

관점 나누기 : [BERTTopic](https://maartengr.github.io/BERTopic/index.html) 모델을 한국어 데이터로 학습한 모델 활용 


