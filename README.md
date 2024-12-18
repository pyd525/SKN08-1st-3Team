# SKN08-1st-3Team

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,70:003300,100:00FF00&height=240&text=SKN01-4th-1Team&animation=&fontColor=00FF00&fontSize=90" width="1000" />
  
  <img width="1000" alt="image" src="https://github.com/Jh-jaehyuk/Jh-jaehyuk.github.io/assets/126551524/7ea63fc3-95f0-44d5-a0f0-cf431cae34f1"> 
  
  [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/SKNETWORKS-FAMILY-AICAMP/SKN01-4th-1Team&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
</div>



# 0. Introduction Team (팀 소개)
### ✅ 팀명 : NC🐘(Nose Childs)
<table align=center>
  <tbody>
    <tr>
      <td align=center><b>양의정</b></td>
      <td align=center><b>유제나</b></td>
      <td align=center><b>박예닮</b></td>
      <td align=center><b>정현서</b></td>
    </tr>
    <tr>
      <td align="center">
        <div>
          <img src="https://avatars.githubusercontent.com/u/100367503?v=4"width="200px; alt="양의정"/>
        </div>
      </td>
      <td align="center">
        <div>
          <img src="https://avatars.githubusercontent.com/u/167101468?v=4"width="200px;" alt="유제나"/>
        </div>
      </td>
      <td align="center">
        <img src="https://avatars.githubusercontent.com/u/188152811?v=4"width="200px;" alt="박예닮"/>
      </td>
      <td align="center">
        <img src="https://avatars.githubusercontent.com/u/122842851?v=4"width="200px;" alt="정현서"/>
      </td>
    </tr>
    <tr>
      <td><a href="https://github.com/UiJungYang"><div align=center>@UiJungYang</div></a></td>
      <td><a href="https://github.com/denalog"><div align=center>@denalog</div></a></td>
      <td><a href="https://github.com/pyd525"><div align=center>@pyd525</div></a></td>
      <td><a href="https://github.com/jungs0914"><div align=center>@jungs0914</div></a></td>
    </tr>
  </tbody>
</table>
  
  
  
# 1. Introduction Project (프로젝트 개요)

### ✅프로젝트 명
차량 DB 조회

### ✅프로젝트 소개
전국 자동차 등록 현황 및 기업 FAQ 조회 웹앱

이 프로젝트는 다양한 자동차 관련 웹사이트에서 차량 등록 현황 및 정보를 크롤링하여 데이터를 수집하고, 
이를 기반으로 데이터를 시각화 및 분석하며, 웹앱 사용자에게 직관적인 UI로 제공하는 시스템입니다. 
특히, Streamlit 기반의 대화형 웹 애플리케이션을 통해 사용자가 데이터를 간편하게 탐색할 수 있도록 설계되었습니다.

### ✅프로젝트 필요성(배경) 
1. **데이터 관리 및 효율화**: 차량 관련 정보를 체계적으로 수집하고, 잘못된 데이터를 쉽게 수정할 수 있어 데이터 관리의 정확성과 효율성을 높입니다.  
2. **분석 및 의사결정 지원**: 지역별 차량 등록 정보와 기업별 충전 요금 데이터를 시각화 및 분석하여 정책 수립, 시장 전략, 인프라 개선 등에 필요한 유용한 통찰을 제공합니다.  
3. **전기차 보급 및 충전 인프라 최적화**: 전기차 등록 현황과 충전 요금 데이터를 통해 지역별 전기차 보급 현황과 충전소 배치의 효율성을 확인하고 개선할 수 있습니다.  
4. **사용자 친화적인 정보 제공**: Streamlit UI를 통해 데이터를 직관적이고 간단하게 시각화하여, 비전문가도 쉽게 정보를 이해하고 활용할 수 있도록 지원합니다.
   
## 비동기 통신 방식의 Deep Learning Local Server
### Syncronous Communication
- 동기(Syncronous)란 동시에 일어난다는 뜻입니다. 즉, Request와 Response가 동시에 일어나는 통신 방식입니다.
- 노드 A와 노드 B 사이의 작업 처리 단위를 동시에 맞춥니다.
- 요청한 결과가 그 자리에서 동시에 주어집니다.
### Asyncronous Communication
- 비동기(Asyncronous)란 동시에 일어나지 않는다는 뜻입니다. 즉, Request와 Response가 동시에 일어나지 않는 통신 방식입니다.
- 노드 사이의 작업 처리 단위를 동시에 맞추지 않겠다는 것으로, 요청한 결과가 그 자리에서 주어지지 않습니다.
### 각 통신 방식의 장단점
- 동기 통신의 경우 설계가 간단하며, 직관적이지만 그 작업이 끝날 때까지 아무런 작업도 할 수 없다는 단점이 있습니다.
- 비동기 통신의 경우 동기 통신보다 비교적 복잡한 구현이 필요하지만, 작업이 끝날 때 까지 기다리지 않아도 되기 때문에 그 동안 다른 작업을 수행할 수 있으므로 효율적인 자원의 사용이 가능합니다.
### 비동기 통신 방식 DLLS
- 모델이 Request에 따라 Response를 하기까지 입력에 대한 결과를 추론하는데에 시간이 필요합니다. 만약 Response를 반환하는 과정을 동기 통신 방식으로 구현한다면, 결과 반환이 완료될 때 까지 사용자는 아무것도 하지 못합니다.
- 따라서, 모델이 추론하여 Response를 반환하는 과정을 비동기 방식으로 설계하여 사용자가 추론 요청 이외의 작업을 수행할 때에도 문제가 없도록 하였습니다.
### 물리적 로컬 서버 구현 이유
- AWS 상에서 LLM 모델의 Fine Tuning 및 추론 과정을 구동시킬 경우, 예산을 넘어서는 비용이 발생할 가능성이 존재합니다.
- 이에 컴퓨팅 자원이 많이 필요한 부분을 따로 물리적 로컬 서버에서 구동하여 Response를 반환하도록 설계하였습니다.
- 결과적으로, 모델 서빙 역할의 FastAPI와 DLLS 상의 AI Client 사이의 비동기 통신을 통해 비용적인 측면에서의 최적화를 달성하고 사용자가 서비스를 사용함에 있어서 불편함이 없도록 하였습니다.
### TLS/SSL 보안 통신 환경 구축
- 커스텀 서버 특성 상, 비교적 해킹에 취약할 가능성이 존재합니다. 이에 보안 프로토콜을 적용하여 외부에서 우리의 서비스에 접근할 수 없도록 보안 통신 환경을 구축하였습니다.

### ✅프로젝트 목표
1. **데이터 수집 및 관리 자동화**: 차량 정보를 효율적으로 크롤링하고 잘못된 데이터를 자동으로 수정할 수 있는 시스템 구축.  
2. **정보 시각화 및 분석 제공**: 지역별 차량 등록 현황 및 기업별 충전 요금을 시각화하여 사용자에게 유용한 데이터를 제공.  
3. **사용자 친화적 인터페이스 개발**: Streamlit 기반 UI를 통해 데이터를 쉽게 조회하고 이해할 수 있는 환경 제공.  
4. **전기차 인프라 최적화 지원**: 데이터 분석을 통해 전기차 보급 및 충전 인프라 관련 정책 수립과 개선에 기여.  



# 2. Tech Stack (기술 스택)

>### <span style="color:cyan"> Co-Work Tool </span>
<table>
  <tr>
    <td>Communication & Messenger</td>
    <td><img src="https://img.shields.io/badge/Discord-5865F2?style=flat&logo=Discord&logoColor=white"/></td>
    <td><img src="https://img.shields.io/badge/Notion-000000?style=flat&logo=Notion&logoColor=white"/></td>
    <td><img src="https://img.shields.io/badge/Slack-4A154B?style=flat&logo=Slack&logoColor=white"/></td>
  </tr>
  <tr>
    <td>Development & Merge</td>
    <td><img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=Git&logoColor=white"/></td>
    <td><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=GitHub&logoColor=white"/></td>
    
</table>

>### <span style="color:cyan"> Frontend </span>
<table>
  </tr>
  <tr>
    <td>Markup & Style & JS</td>
    <td><img src="https://img.shields.io/badge/HTML-E34F26?style=flat&logo=html5&logoColor=white"/></td>
    <td><img src="https://img.shields.io/badge/css-1572B6?style=flat&logo=css3&logoColor=white"/></td>
</table>

>### <span style="color:cyan"> Backend </span>
<table>
  <tr>
    <td>BE IDE & Language</td>
    <td><img src="https://img.shields.io/badge/pycharm-%23000000?style=flat&logo=pycharm&logoColor=white"/></td>
    <td><img src="https://img.shields.io/badge/python-3776AB?style=flat&logo=python&logoColor=white"/></td>
  </tr>  
  <tr>
    <td>RDBMS</td>
    <td><img src="https://img.shields.io/badge/mysql-4479A1?style=flat&logo=mysql&logoColor=white"/></td>
    <td></td>
  </tr>
  
</table>
<br><br><br>



# 3. 시스템 구성도
![image](https://github.com/user-attachments/assets/66a78240-b41d-487a-8800-29bccbab7d41)
<br><br><br>



## 애자일 보드를 사용하는 이유
```c
과거 정의서들을 일일히 작성하였지만 빠른 속도로 무언가를 개발하는데 한계가 있습니다.
처음부터 많은 것들을 빌드업하면서 빠른 생산성을 기반으로 움직이려면 반드시 애자일해야합니다.
고로 폭포수 설계 방식이 아닌 애자일 프로세스 방식으로 애자일 보드를 작성하면서 진행했습니다.

애자일 보드는 자체적으로 제목이 요구 사항을 내포하며 각 카드 내부에는 정의한 Domain의 세부 사항이 기록됩니다.
고로 빠르게 팀원들과 협업 할 수 있고 소통 비용을 최소화시킬 수 있습니다.
작은 것 같지만 이와 같은 것들이 쌓여서 아주 기민하고 민첩한 조직을 만들어 냅니다.
```
# 4. 애자일 보드
![image](https://github.com/user-attachments/assets/3a004f06-79ca-4969-ac43-419d35f588c1)
![image](https://github.com/user-attachments/assets/1067094c-efa8-40f3-9c72-8742af0a5160)


# 5. 비용 최적화를 위한 Deep Learning Local Server 구성 + 보안 설정을 위한 TLS / SSL 소켓 구성
### 5-1 Socket Server (FastAPI) 구성 및 구동 방법
(1) FastAPI 프로젝트 폴더 내에서 미리 구성해 놓은 소켓 통신 관련 submodule을 다음의 명령어를 통해 연결합니다.
```bash
git submodule add "socket server submodule Github 주소" template
```

(2) 다음과 같이 `template` 라는 submodule이 프로젝트 내부에 붙은 것을 확인할 수 있습니다.
![image](https://github.com/user-attachments/assets/fc83fd3b-3cf0-4852-a6e1-c143afb3eed3)
(3) 이후에 `cd include/socket_server/`에 소켓 서버의 역할을 하도록 해놓은 모듈에 대한 내용들을 다음의 명령어로 갱신시킵니다.
![image](https://github.com/user-attachments/assets/1bf1190e-1aad-45d9-ad6b-d44090f88c0f)
```bash
cd ../..
git submodule update --init --recursive
```
(4) 그러면 아래처럼 내용들이 추가된 것을 확인할 수 있습니다.
![image](https://github.com/user-attachments/assets/bb624477-e11a-461c-a532-63389108c566)

(5) 이후 미리 준비해놓은 보안 관련 파일들을 프로젝트 폴더에 배치시킵니다.
```bash
CA.pem
svr.key
svr.crt
```

(6) 서버를 구동시키면 다음과 같이 ai-client의 접속을 대기하는 것을 확인할 수 있습니다.
![image](https://github.com/user-attachments/assets/dbdf40fe-1fc0-4e15-9c05-73618d202e63)

### 5-2 Socket Client (ai-client) 구성 및 구동 방법
(1) ai-client 프로젝트 폴더 내에서 소켓 서버와 마찬가지로 미리 구성해 놓은 소켓 통신 관련 submodule을 다음의 명령어를 통해 연결합니다.
```bash
git submodule add "socket client submodule Github 주소" template
```

(2) 다음과 같이 `template` 라는 submodule이 프로젝트 내부에 붙은 것을 확인할 수 있습니다.
![image](https://github.com/user-attachments/assets/7340470c-97c3-4ee4-ab18-d52bbc6a8c83)

(3) 이후 미리 준비해놓은 보안 관련 파일들을 프로젝트 폴더에 배치시킵니다.
```bash
CA.pem
client.key
client.crt
```

(4) 서버를 구동시킨 상태에서 ai-client를 구동하여 socket server로 접속을 시도하면 다음과 같이 잘 접속되는 것을 확인할 수 있습니다. 또한, 미리 구성한 보안 접속도 잘 작동하는 것을 확인할 수 있습니다.
![image](https://github.com/user-attachments/assets/98fdf151-ee23-41ba-a09d-fc1ac6ffd2d0)


# 6. 데이터 전처리

## 벡터 저장소
검색 속도 향상을 위해, FAISS를 사용하여 벡터 저장소를 생성 및 저장합니다. 
<br>FAISS를 사용하기 위해 텍스트를 청크 단위로 나눈 후 Document 형태로 변환합니다.

```python
def splitTextIntoDocuments(self, text, chunkSize=256, chunkOverlap=16):
    textSplitter = RecursiveCharacterTextSplitter(chunk_size=chunkSize, chunk_overlap=chunkOverlap)
    chunkList = textSplitter.split_text(text)

    documentList = [Document(page_content=chunk) for chunk in chunkList]
    return documentList
```
이후, 임베딩을 통해 벡터화를 진행한 뒤 FAISS를 사용하여 벡터 저장소를 생성하고 저장합니다.

```python
def createFAISS(self, documentList):
    embeddings = OpenAIEmbeddings()

    vectorstore = FAISS.from_documents(documentList, embeddings)
    print("success to create VectorStore")

    return vectorstore

def saveFAISS(self, vectorstore, dbPath):
    vectorstore.save_local(dbPath)
```

## TF-IDF 기반의 벡터 산출
사용자로부터 논문 요약을 요청받았을 때, 전체 텍스트를 모두 사용하는 것은 비효율적일 수 있기 때문에 텍스트의 길이를 줄이는 추가적인 작업이 필요합니다.
<br>먼저, 텍스트를 문장 단위로 나누고 TF-IDF 벡터를 생성합니다.
```python
sentences = sent_tokenize(mainText)

vectorizer = TfidfVectorizer().fit_transform(sentences)
vectors = vectorizer.toarray()
```
문장 간 유사도 행렬을 계산하고, 그 기반으로 그래프를 생성합니다.
```python
similarityMatrix = cosine_similarity(vectors)

nxGraph = nx.from_numpy_array(similarityMatrix)
scores = nx.pagerank(nxGraph)
```
점수에 따라 문장을 정렬한 뒤, 사용할 문장의 수를 잘 설정하여 선택합니다.
```python
rankedSentences = sorted(((scores[i], s) for i, s in enumerate(sentences)), reverse=True)
top_n = 100
rankedText = " ".join([sentence for score, sentence in rankedSentences[:top_n]])
```

# 7. 모델
LLama3.0, LLama3.1, OpenAI API 등 여러 모델을 사용해 보고, 입력 토큰 수와 추론 속도를 고려하여
<br>최종적으로 OpenAI의 gpt-4o-mini 모델을 선택하고, LangChain을 활용했습니다.

## Basic
LLM과 프롬프트 템플릿을 연결하여 체인을 만들고, 사용자가 보낸 메시지(userSendMessage)를 받아 question 변수에 해당하는 값으로 프롬프트 템플릿에 적용하고, 이를 통해 LLM이 텍스트를 생성하는 작업을 실행합니다.
```python
llm = ChatOpenAI(temperature=0.3, model_name="gpt-4o-mini")
prompt_template = PromptTemplate(
    input_variables=["question"],
    template=template
)

chain = LLMChain(llm=self.llm, prompt=prompt_template)
return {"generatedText": chain.run(userSendMessage)}
```

## 질의 응답
논문 관련 질의응답 시, LLM의 단점인'사실 관계 오류 가능성'과 '맥락 이해의 관계'를 개선하기 위해 RAG(Retrieval-Augmented Generation)를 사용했습니다.
<br>LangChain을 사용하여 RAG 체인을 구성하고, 사용자의 입력을 처리한 후 그에 대한 답변을 생성합니다.
<br>LangChain 허브에서 프롬프트를 불러온 뒤, RAG체인을 구성합니다. RAG는 외부 데이터를 검색하고, 이를 LLM을 통해 답변을 생성하는 방식으로 동작합니다.
<br>vectorstore.as_retriever()를 통해 전처리 과정에서 생성된 FAISS 벡터 저장소에서 문서를 검색하고, 사용자의 입력과 유사한 문서를 결과로 반환합니다.
```python
def format_docs(docs):
    return "\n\n".join([doc.page_content for doc in docs])

userSendMessage = fileKey.split(".")[0] + " " + userSendMessage
prompt = hub.pull("godk/korean-rag", api_key=langchain_api_key)

rag_chain = (
    {"context": vectorstore.as_retriever() | format_docs, "question": RunnablePassthrough()}
    | prompt
    | self.llm
    | StrOutputParser()
)
return {"generatedText": rag_chain.invoke(userSendMessage)}
```

## 요약
마찬가지로 LLM 체인을 생성하고 여러 문서를 하나의 텍스트로 채워넣는 StuffDocumentsChain을 정의합니다. 전처리 과정으로 줄여진 문서화된 텍스트가 실제 Input에 해당합니다.
<br>StuffDocumentsChain을 통해 문서 내용을 프롬프트에 삽입한 후, LLM을 사용해 요약을 생성하고, 그 결과를 반환합니다.
```python
docs = [Document(page_content=rankedText, metadata={})]
prompt_template = """실제로 프롬프트가 작성되어 있지만 생략하겠습니다.
"""
prompt = PromptTemplate.from_template(prompt_template)
llm_chain = LLMChain(llm=self.llm, prompt=prompt)

stuff_chain = StuffDocumentsChain(llm_chain=llm_chain, document_variable_name="context")
output = stuff_chain.invoke({"input_documents": docs})
return {"generatedText": output["output_text"]}
```


# 8. Result (수행 결과)

### ✅ PostMan 결과
![image](https://github.com/user-attachments/assets/66107076-2e88-4354-bd3a-d184c9ffa312)
![image](https://github.com/user-attachments/assets/2c373fae-ef69-4731-b7bb-f8cabc370438)
![image](https://github.com/user-attachments/assets/0201f50d-1a61-4f27-a365-4b3a71dd4748)
![image](https://github.com/user-attachments/assets/392a1097-8016-4cd9-8177-214cb843dec9)

### ✅ SQL 동작 확인: MySQL 데이터베이스에서 데이터를 정확히 삽입하고 가져오는 기능이 정상적으로 작동함을 확인했습니다.
![image](https://github.com/user-attachments/assets/8ce37889-8a67-4ae5-8585-c2210fd84f2c)
![image](https://github.com/user-attachments/assets/4ad7156f-38e1-495d-bcfc-4982eb2a528a)
![image](https://github.com/user-attachments/assets/600e565e-d874-4764-9197-cf38bdc2bcc3)
![image](https://github.com/user-attachments/assets/d7c9c2a9-9cdf-4305-aee7-e91bbf184157)


### ✅ 데이터 크롤링 성공: 주요 자동차 등록 정보를 제공하는 웹사이트로부터 데이터를 성공적으로 크롤링하여 MySQL 데이터베이스에 저장하였습니다.
![image](https://github.com/user-attachments/assets/8aecd593-11ed-4325-ac2b-282e0f1cc977)
![image](https://github.com/user-attachments/assets/5b63c972-38ac-4c28-9e61-ff486701bf9d)
![image](https://github.com/user-attachments/assets/761dbbee-f4c5-4a28-a90a-4f59b31d1132)

<br><br><br>

  
# 9. 한 줄 회고
🤓<b>양의정</b>  
_👏크롤링을 통해 데이터를 수집하고 데이터베이스에 저장한 정보를 한눈에 볼 수 있는 사이트를 만들었습니다. 이 프로젝트를 통해 개발이 이런 것이구나를 느낄 수 있는 기회였습니다.👏_

👨‍💻<b>유제나</b>  
_😍데이터를 크롤링하고 MySQL 데이터베이스에 연동하며 데이터 수집부터 저장, 처리, Streamlit을 활용한 시각화까지 전 과정을 직접 다뤄볼 수 있어 유익한 경험이었습니다. 이 과정을 통해 데이터 활용의 흐름을 이해할 수 있었습니다.😍_

😺<b>정현서</b>  
_첫 팀프로젝트라 여러 어려움이 있었지만, 그래도 무사히 마칠 수 있어 다행이라고 생각합니다. 팀원들 모두 고생하셨습니다.😊_

🪐<b>박예닮</b>  
_해보고 느낀건 아직은 많이 미숙한거같습니다 열심히해야될거같습니다 미안합니다 사랑합니다 감사합니다._

