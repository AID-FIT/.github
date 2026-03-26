# 👕 프로젝트 : AID-Fit (Intelligent Fashion Agent)

**"사용자의 스타일을 '보고' 맥락을 '이해'하여 최적의 코디를 '제안'하는 지능형 패션 에이전트"**
---

## 1. 프로젝트 개요 및 목표
* **개요:** 사용자의 시각적 정보(VLM)와 지식 베이스(RAG)를 바탕으로, 지능형 에이전트가 상황(TPO)에 맞는 최적의 코디를 제안하는 서비스.
* **핵심 목표:**
* 1. **Agentic Logic:** 단순 추천을 넘어 '왜 이 옷인가'에 대한 논리적 추론 제공.
* 2. **Seamless Integration:** 비전, 검색, 생성 모델의 매끄러운 통합 파이프라인 구축.
* 3. **User-Centric UI:** AI의 복잡한 추론 과정을 사용자에게 직관적으로 전달.

---

## 2. 팀원 역할 분담 (Roles)

| 성명/역할 | 주요 책임 (Responsibilities) | 핵심 작업 (Tasks) |
| :--- | :--- | :--- |
| **Member A**<br>(Full-stack / Integrator) | **시스템 구현 및 인터페이스 통합** | - **FE:** React/Flutter/RN 기반 UI/UX 구현<br>- **BE:** FastAPI 서버 구축 및 API 엔드포인트 설계<br>- **통합:** B, C, D의 모듈을 연결하는 파이프라인 연동 |
| **Member B**<br>(Data / RAG) | **지식 베이스 및 검색 시스템** | - 의류 데이터셋 확보 및 전처리 (Cleaning)<br>- Vector DB (ChromaDB/FAISS) 구축<br>- 유사도 검색(Similarity Search) 최적화 |
| **Member C**<br>(Vision / VLM) | **시각 데이터 분석 및 정형화** | - VLM (GPT-4o/Gemini) 프롬프트 최적화<br>- 이미지 특징(색상, 소재, 핏, 무드) 추출 로직<br>- 추출 데이터의 JSON 파싱 자동화 |
| **Member D**<br>(Agent / Strategist) | **에이전트 설계 및 추론 로직** | - **에이전트 설계:** LangChain/LangGraph 기반 워크플로우 구축<br>- **코디 추론:** TPO/개인 취향에 따른 논리 엔진 개발<br>- **가이드 생성:** 환각 제어 및 개인화된 스타일링 가이드 출력 |

---

## 3. 3개월 핵심 마일스톤 (Roadmap)

### **1개월 차: 기초 구축 및 기술 검증 (PoC)**
- 프로젝트 환경 설정 및 협업 툴(Git, Notion) 세팅
- 의류 데이터셋 확보 및 Vector DB 초기 설계
- VLM 및 LLM API 연동 테스트 및 성능 벤치마킹
- UI 와이어프레임 확정

### **2개월 차: 핵심 로직 구현 (MVP)**
- VLM-RAG-LLM 파이프라인 단일 흐름 연결
- 이미지 특징 추출 프롬프트 고도화 및 JSON 파싱 자동화
- 백엔드 API 서버와 프론트엔드 연동
- 에이전트 도구(Tool) 호출 및 라우팅 로직 구현

### **3개월 차: 고도화 및 최종 결과물 도출**
- 추천 결과의 정확도 향상을 위한 리랭킹(Re-ranking) 적용
- 예외 상황(이미지 분석 실패 등) 처리 및 시스템 안정화
- 최종 UI 디자인 입히기 및 성능 최적화(응답 속도 개선)
- 최종 시연 영상 제작 및 프로젝트 문서화 마무리

---

## 🛠 기술 스택 (Tech Stack)
* **LLM/VLM:** GPT-4o-mini, Gemini 1.5 Flash
* **Framework:** LangChain, FastAPI, React/Flutter
* **Database:** ChromaDB (Vector Store), PostgreSQL (Metadata)
* **Infrastructure:** Firebase (Storage/Alert), Docker (Optional)

---
