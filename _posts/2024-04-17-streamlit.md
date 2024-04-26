---
layout: single
title:  Streamlit 사용방법 및 실시간 상호작용하기 와 종료방법 (VSC)
excerpt: Streamlit
categories: AWS # 카테고리 설정하기 
tags: [AWS, Study] # 태그 설정하기 
author_profile: false
toc: true # 목차 활성화 
toc_sticky: true # 목차 따라다니게 하는 기능 추가
toc_label: "목차" # 목차 이름 설정하기 
toc_icon: "fas fa-star" # 목차 아이콘 설정 
comments: ture  # 댓글 활성화 \
author_profile: True
sidebar:
    nav: "main"
---

# 1. Streamlit이란?

- 앱을 구축하고 공유하는 프레임워크
- Python 으로 데이터 앱을 빠르고 쉽게 만들수 잇도록 돕는 오픈 소스 앱 프레임워크
- 즉 웹, 대시보드를 생성하여 이와 상호작용을 가능하게 만들어 주는것이다.


# 2. VSC(Visual Studio Code)를 사용하여 Streamlit 사용하기

# 2-1. Streamlit 라이브러리를 호출하여 사용
- 웹 대시보드를 생성하여 문구 출력하기

```python

import streamlit as st # 스트림릿 라이브러리를 사용하기 위한 임포트이다.

# 웹 대시보드 개발 라이브러리인 스트림릿은 main 함수가 있어야 하기때문에 def 함수를 사용하여 만들어준다.
def main() :
    st.title('웹 대시보드 프로젝트')
    st.title('test')

if __name__ == '__main__' :
    main()
```

## 소스코드 if__name__ == '__main__' 는 무엇일까?
- 그대로 해석해보면 'name이라는 변수의 값이 main일때 아래의 코드를 실행하라' 라는 의미이다.
- 즉, 메인 함수의 선언, 시작을 의미하며, 현재 스크립트 파일이 실행되는 상태를 파악하기 위해 사용한다.
- 스크립트 파일이 프로그램의 시작점이 맞는지 판단하는 작업이며, 스크립트 파일이 메인 프로그램으로 사용될 때와 모듈로 사용될 때를 구분하기 위한 용도이다.
- 쉽게 생각하면 모듈에 if__name__ == '__main__' 이라는 조건문을 넣어준뒤 그 아래는 직접 실행시켰을 때만 실행되길 원하는 코드들을 넣어주는것이다.   

자세한 설명 보러가기 : [설명보기](https://velog.io/@mjk3136/if-name-main%EC%9D%80-%EC%99%9C-%ED%95%84%EC%9A%94%ED%95%9C%EC%A7%80%EC%97%90-%EB%8C%80%ED%95%B4-%EC%95%8C%EC%95%84%EB%B3%B4%EC%9E%90){: .btn .btn--primary}  

# 2-2. VSC에서 터미널 사용하기
1. 상단의 Terminal 탭 => New Terminal
<img src="/images/a.png">

2. 하단의 + 표시 클릭 => Command Prompt
<img src="/images/aa.png">

# 2-3. Streamlit 실행하기
1. 하단 TERMINAL 에서 'cmd' 선택
2. streamlit run 파일명(준비한 파일) 입력 [이때 파일명은 .py로 끝나야한다.]

