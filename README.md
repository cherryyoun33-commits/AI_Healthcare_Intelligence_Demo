# AI Healthcare Intelligence Platform

## From Healthcare Knowledge to Clinical Intelligence

**A personal AI-powered knowledge operating system for healthcare AI research.**

의료 AI 논문, 임상 가이드라인, 정부자료, 연구 메모를 구조화하고 연결하여  
단순한 자료 보관을 넘어 실제 연구와 임상적 인사이트로 발전시키기 위한  
개인용 AI Knowledge Operating System입니다.

---

## Overview

Healthcare AI research produces a large volume of fragmented information across papers, guidelines, reports, datasets, and internal notes.

This project was designed to transform those disconnected materials into reusable knowledge assets.

의료 AI 연구자료는 논문, 가이드라인, 정부 보고서, 데이터셋, 개인 메모 등 여러 형태로 흩어져 있습니다.

이 프로젝트는 이러한 자료를 다음과 같은 흐름으로 전환합니다.

```text
Source Documents
        ↓
Knowledge Objects
        ↓
Learning Notes
        ↓
AI Reflection
        ↓
Connections
        ↓
Semantic Search
        ↓
Grounded QA
        ↓
Research Insights
```

---

## What This Platform Does

### Knowledge Objects

논문, 가이드라인, 보고서 등 서로 다른 형식의 자료를 일관된 구조의 Knowledge Object로 변환합니다.

주요 항목:

- Metadata
- Dashboard Summary
- Overview
- Key Findings
- Platform Relevance
- Current MVP Relevance
- Evidence and Resources

### Learning Notes

복잡한 연구자료를 다시 학습할 수 있도록 핵심 개념, 질문, 적용 포인트 중심의 학습 노트로 변환합니다.

### AI Reflection

단순 요약을 넘어 다음 관점에서 자료를 해석합니다.

- 의료 AI 플랫폼 적용 가능성
- 현재 MVP와의 연관성
- 연구 공백
- 제품 아이디어
- 후속 연구 질문

### Connections

서로 다른 논문, 가이드라인, 내부 메모 사이의 관계를 연결합니다.

예:

```text
Paper
  ↓ supports
Clinical Guideline
  ↓ informs
MVP Architecture
  ↓ generates
Implementation Decision
```

### Semantic Search

키워드가 정확히 일치하지 않아도 의미적으로 관련된 자료를 탐색할 수 있습니다.

### Grounded Question Answering

저장된 자료와 Evidence Span을 기반으로 질문에 답변하도록 설계했습니다.

답변에는 가능한 경우 다음 정보를 연결합니다.

- Source document
- Evidence span
- Related knowledge object
- Relevant section
- Supporting context

### Study Assist

논문이나 전문 자료의 어려운 부분을 더 쉽게 이해할 수 있도록 설명합니다.

### Personal Notes and Reflection

사용자가 작성한 메모와 AI가 생성한 분석을 분리하여 관리합니다.

---

## Why This Is Not Just a Chatbot

This project is not designed as a simple conversational interface.

It is designed as a persistent research environment where knowledge can be accumulated, reviewed, connected, and reused over time.

이 프로젝트는 일회성 질문에 답하는 챗봇이 아닙니다.

다음과 같은 지속 가능한 연구 환경을 만드는 것이 목표입니다.

- 자료를 구조적으로 축적
- 근거와 출처를 보존
- 문서 간 관계를 연결
- 학습 결과를 재사용
- 새로운 연구 질문을 생성
- 임상 AI MVP 설계로 연결

---

## Current Features

| Feature | Description |
|---|---|
| Knowledge Ingestion | 논문, 가이드라인, 보고서, 내부 지식 수집 |
| Knowledge Objects | 구조화된 지식 객체 생성 |
| Learning Notes | 학습용 노트 자동 생성 |
| AI Reflection | 플랫폼 및 MVP 관점의 해석 |
| My Notes | 사용자 메모 관리 |
| Connections | 지식 간 관계 생성 |
| Semantic Search | 의미 기반 검색 |
| Grounded QA | 근거 기반 질의응답 |
| Evidence Deep Link | 답변 근거 위치 연결 |
| Study Assist | 어려운 내용을 쉽게 설명 |
| Batch Ingestion | 여러 문서 일괄 처리 |
| Crash-safe Logging | 배치 처리 중 실시간 진행 로그 저장 |
| Dashboard | 지식 탐색과 검토를 위한 웹 인터페이스 |

---

## Supported Knowledge Types

| Type | Prefix | Description |
|---|---:|---|
| Paper | P | Academic research papers |
| Government | G | Government and public institution reports |
| Report | RP | Strategic and industry reports |
| Guideline | GL | Clinical and professional guidelines |
| Company | C | Company documents |
| Benchmark | B | Benchmarks and evaluation resources |
| Dataset | D | Datasets |
| Product | PR | Digital health and AI products |
| Regulation | R | Regulations and policy documents |
| News | N | Relevant news |
| Internal Knowledge | KB | Internal notes and synthesized knowledge |

---

## System Architecture

```text
Document Sources
    │
    ▼
Ingestion Pipeline
    │
    ├── Document Type Detection
    ├── Text Extraction
    ├── Metadata Generation
    ├── Knowledge Object Generation
    └── Repository Registration
    │
    ▼
Knowledge Layer
    │
    ├── Knowledge Objects
    ├── Learning Notes
    ├── AI Reflection
    ├── My Notes
    └── Connections
    │
    ▼
Retrieval Layer
    │
    ├── Chunking
    ├── Embeddings
    ├── Semantic Search
    └── Evidence Retrieval
    │
    ▼
Application Layer
    │
    ├── Dashboard
    ├── Grounded QA
    ├── Study Assist
    └── Evidence Deep Links
```

---

## Technology Stack

### Backend

- Python
- FastAPI
- Pydantic
- Pytest

### Frontend

- React
- TypeScript
- Vite

### AI and Retrieval

- Large Language Models
- Prompt-based structured generation
- Embeddings
- Semantic retrieval
- Evidence-grounded question answering

### Development and Operations

- Git
- GitHub
- Automated tests
- Architecture Decision Records
- Crash-safe batch logging

---

## Quality and Safety Principles

### Evidence First

중요한 주장과 답변은 가능한 경우 근거 문서와 Evidence Span에 연결합니다.

### No Unsupported Inference

자료에 없는 내용을 확정적으로 생성하지 않도록 설계합니다.

### Human Review

AI가 생성한 결과는 최종 판단이 아니라 검토 가능한 지식 후보로 취급합니다.

### Source Separation

원본 자료, 구조화 산출물, 사용자 메모, AI 분석 결과를 구분하여 관리합니다.

### Repository Protection

원본 PDF와 전체 번역본은 공개 저장소에 포함하지 않습니다.

Private 개발 저장소와 Public Demo 저장소를 분리하여 운영합니다.

---

## Current Project Status

```text
Knowledge Objects        190+
Automated Tests          450
Production Build         Passed
Repository Protection    Verified
Batch Logging            Implemented
Semantic Retrieval       Implemented
Grounded QA              Implemented
Study Assist             Implemented
```

수치는 프로젝트 진행에 따라 달라질 수 있습니다.

---

## Related Clinical AI Direction

This knowledge platform also supports the design of a separate clinical AI MVP.

The related MVP explores how patient free-text symptom messages can be transformed into structured clinical information and evidence-linked clinician review support.

이 플랫폼에서 축적한 지식은 별도의 임상 AI MVP 설계에도 활용됩니다.

현재 관련 프로젝트에서는 다음 흐름을 연구하고 있습니다.

```text
Patient Free-text
        ↓
Symptom Structuring
        ↓
Safety Review
        ↓
Follow-up Question
        ↓
Clinical Context Integration
        ↓
Guideline Retrieval
        ↓
Evidence-linked Clinician Review
```

---

## Demo Repository Scope

This public repository is intended only for demonstration and portfolio purposes.

공개 저장소에는 다음 내용만 포함합니다.

- 프로젝트 소개
- 공개 가능한 화면
- 아키텍처 설명
- 샘플 데이터
- 제한된 데모 기능

다음 내용은 포함하지 않습니다.

- 원본 논문 PDF
- 전체 번역본
- 개인 연구 데이터
- 비공개 Knowledge Base
- API Key
- 개인 사용 기록
- 내부 실험 자료

---

## Roadmap

### Near Term

- Public dashboard demo
- Curated sample knowledge objects
- Architecture visualization
- Improved onboarding
- Demo-friendly search experience

### Mid Term

- Knowledge graph visualization
- Research theme clustering
- Citation-aware synthesis
- Automated evidence quality checks
- Multi-document comparative analysis

### Long Term

- Clinical AI knowledge workflow
- Structured symptom intelligence
- Guideline-aware decision support
- Research-to-product knowledge lifecycle

---

## Disclaimer

This project is a personal research and prototyping environment.

It is not a medical device and does not provide diagnosis, treatment decisions, or direct patient care instructions.

이 프로젝트는 개인 연구 및 프로토타이핑 목적으로 제작되었습니다.

의료기기, 진단 시스템, 치료 권고 시스템 또는 직접적인 환자 진료 도구가 아닙니다.

---

## Author

Developed as a personal healthcare AI research project.

Clinical workflow, quality improvement, digital health, and AI product design perspectives are reflected in the project architecture.
