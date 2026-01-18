# Argo CD Kubernetes GitOps

## 📌 Overview
이 저장소는 **Argo CD를 활용한 Kubernetes GitOps 자동 배포 구성**을 담은 리포지토리입니다.  
Git 저장소에 선언된 Kubernetes 매니페스트(YAML)를 기준으로, Argo CD가 클러스터 상태를 자동으로 동기화하여 지속적인 배포(Continuous Delivery)를 구현합니다.

GitHub 저장소의 YAML을 수정하고 커밋하면, 별도의 수동 배포 없이 Argo CD가 이를 감지하여 Kubernetes 클러스터에 자동 반영하도록 구성할 수 있습니다.

---

## 🧩 Architecture (GitOps Flow)

```
GitHub Repository (YAML)
          ↓
        Argo CD
          ↓
   Kubernetes Cluster
```

- Git을 **단일 진실 공급원(Single Source of Truth)** 으로 사용
- Argo CD가 선언적 매니페스트를 지속적으로 감시 및 동기화
- 수동 배포 작업 최소화 및 배포 안정성 향상

---

## 📂 Repository Structure
```
.
├── README.md
├── vnc/
│   ├── deployment-vncserver.yaml    # VNC 서버 Deployment 정의
│   └── service-vncserver.yaml       # VNC 서버 Service 정의
└── .gitignore
```

- `vnc/` 디렉터리는 Argo CD 동기화 테스트를 위한 **샘플 애플리케이션 배포 매니페스트**입니다.

---

## ⚙️ Prerequisites
- Kubernetes Cluster (온프레미스 / 퍼블릭 클라우드)
- kubectl 설정 완료
- Argo CD 설치 환경

---

## ✅ What This Project Demonstrates
- GitOps 기반 Kubernetes CD 자동화 이해
- Argo CD Application 구성 및 동기화 경험
- 선언적(Declarative) 인프라 관리 방식 숙련
- Git → Argo CD → Kubernetes 배포 흐름 실습

---

