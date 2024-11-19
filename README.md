### API 관련 사항

- Gemini API를 사용하여 실습을 진행하였습니다.
- 따라서 Gemini API key 파일이 필요하므로 아래와 같이 합니다. <br><br>
  1. repository를 clone 합니다. (아래에 적어두었음)
  2. 자신의 API 키를 복사하여 메모장/텍스트 편집기에 붙여넣기합니다.
  3. 붙여넣기한 내용을 저장하는데, 확장자를 `.key` 로 해서 `gemini_api.key` 파일을 만듭니다.
  4. 마지막으로 만든 파일을 clone한 directory의 폴더 최상단에 두면 됩니다.

### 이 Repository를 자신의 컴퓨터로 복사하기 (clone)
git bash 혹은 터미널에 붙여넣기 하면 됩니다.
```
git clone https://github.com/7minseok7/ch3_chatbot_practice.git
```

### 필수과제

`필수과제.ipynb` 에서는 Gemini API를 활용하여 주어진 PDF를 읽고 이 내용을 토대로 챗봇의 기능을 수행하도록 하였습니다.

- 주어진 PDF는 Datasets 디렉토리 안에 있으며 이 파일을 맥락으로 하여 RAG를 수행하게 됩니다.
- 또한 맥락을 주지 않은 일반적인 상황에서의 모델의 출력도 같이 확인할 수 있도록 했습니다.

### 도전과제

`도전과제.ipynb` 에서는 시스템 프롬프트 여러 개에 대하여 같은 사용자 프롬프트에 대해 답변이 어떻게 바뀌는지를 비교해 봅니다.

- 시스템 프롬프트는 Prompts 폴더에 있으며 내부에 있는 txt 파일을 읽고 이것을 LangChain을 통해 시스템 프롬프트로 전달합니다.
- 모델의 출력은 ipynb상에도 출력되지만 Results 폴더에 프롬프트 번호와 현재 시간을 반영하여 저장하도록 했습니다.
