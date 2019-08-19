---
title: "노드 객체 정리"
date: 2019-08-04 17:10:02 -0400
categories: [DOM]
comments: true
tags: [DOM]
---
#노드 객체

#### 노드 객체
- 문서 개체 모델(DOM)은 자바스크립트 Node객체의 계층화된 트리(tree)이다.  
- 브라우저는 HTML 문서 로딩시 계층구조를 해석해서 마크업이 어떻게 캡슐화 되었는지를 보여주는 노드 객체 트리를 생성한다.    
- DOM의 목적은 JavaScript를 이용해 문서에 대한 스트립트 작성(삭제, 추가, 바꾸기, 이벤트 처리, 수정)을 위한 프로그래밍 인터페이스를 제공하는것이다.  
- Node는 여러 가지 DOM 타입들이 상속하는 인터페이스이다. 모든 DOM은 Node로부터 메소드와 프라퍼티를 상속받는다. 상속을 받는 예는 아래와 같다.  

#### 노드 객체의 주요기능
Node 객체의 주요한 임무는 아래와 같다.  

#### 관계
엘리먼트는 서로 부모, 자식, 혹은 형제자매 관계로 연결되어 있다. 각각의 Node가 다른 Node와 연결된 정보를 보여주는 API를 통해서 문서를 프로그래밍적으로 탐색할 수 있다.  

- Node.childNodes
- Node.firstChild
- Node.lastChild
- Node.nextSibling
- Node.previousSibling
- Node.contains()
- Node.hasChildNodes()  

#### 노드의 종류
Node 객체는 모든 구성요소를 대표하는 객체이기 때문에 각각의 구성요소가 어떤 카테고리에 속하는 것인지를 알려주는 식별자를 제공한다.  

- Node.nodeType
- Node.nodeName  

#### 값
Node 객체의 값을 제공하는 API  

- Node.nodeValue
- Node.textContent  

#### 자식관리
Node 객체의 자식을 추가하는 방법에 대한 API  

- Node.appendChild()
- Node.removeChild()  
  
#### 노드 개체 유형
노드 개체의 유형은 <code>Node.nodeName <br>Node.nodeType </code>을 이용해 값을 알 수 있다.  

| Name                        | Value |
|-----------------------------|-------|
| ELEMENT_NODE                | 1     |
| ATTRIBUTE_NODE              | 2     |
| TEXT_NODE                   | 3     |
| CDATA_SECTION_NODE          | 4     |
| ENTITY_REFERENCE_NODE       | 5     |
| ENTITY_NODE                 | 6     |
| PROCESSING_INSTRUCTION_NODE | 7     |
| COMMENT_NODE                | 8     |
| DOCUMENT_NODE               | 9     |
| DOCUMENT_TYPE_NODE          | 10    |
| DOCUMENT_FRAGMENT_NODE      | 11    |
| NOTATION_NODE               | 12    |  

#### 노드 속성 및 메소드
노드를 다루기 위한 속성 및 메소드를 구분해 정리한다.  

##### Node 속성  

- childNodes
- firstChild
- lastChild
- nextSibling
- nodeName
- nodeType
- nodeValue
- parentNode
- previousSibling  

  
##### Node 메소드  

- appendChild()
- cloneNode()
- compareDocumentPosition()
- contains()
- hasChildNodes()
- insertBefore()
- isEqualNode()
- removeChild()
- replaceChild()  

  
##### Documnent 메소드  

- document.createElement()
- document.createTextNode()  

  
##### HTML *Element 속성  

- innerHTML
- outerHTML
- textContent
- innerText
- outerText
- firstElementChild
- lastElementChild
- nextElementChild
- previousElementChild
- children  


##### HTML element 메서드  

- insertAdjacentHTML()  
