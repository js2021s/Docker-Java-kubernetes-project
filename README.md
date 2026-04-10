# Java Microservices: Kubernetes & CI/CD Orchestration
![Java CI/CD with Docker](https://github.com/js2021s/Docker-Java-kubernetes-project/actions/workflows/ci-cd.yml/badge.svg)


Dieses Projekt demonstriert die Modernisierung einer Java-basierten Microservices-Anwendung. Der Fokus liegt auf der Containerisierung, der Orchestrierung mit Kubernetes und der Automatisierung über eine CI/CD-Pipeline.

# Features & Highlights
- Microservices-Architektur: Drei entkoppelte Services (shopfront, productcatalogue, stockmanager).

- Dockerization: Multi-Stage Builds für optimierte und sichere Docker-Images.

- Kubernetes Orchestration: Skalierbare Deployments und stabiles Networking über ClusterIP/NodePort Services.

- CI/CD Automation: Automatisierter Build- und Push-Prozess zu Docker Hub mittels GitHub Actions.

# Technologie-Stack
- Backend: Java 17, Maven

- Container: Docker

- Orchestrierung: Kubernetes (Minikube/K3s)

- Pipeline: GitHub Actions

- Registry: Docker Hub

# Architektur-Workflow
Der Deployment-Prozess folgt dem modernen DevOps-Ansatz:

1. Code Push: Entwickler pusht Code in den main Branch.

2. GitHub Actions: Automatisiertes Bauen der JAR-Dateien und Erstellen der Docker-Images.

3. Docker Hub: Images werden versioniert in der Registry gespeichert.

4. Kubernetes: Deployment der Applikation im Cluster (Self-healing & Scaling).

# Installation & Deployment

1. Lokales Bauen (Docker)
Um die Images manuell zu bauen:    docker build -t js2021s/shopfront:latest ./shopfront

2. Kubernetes Deployment
Navigiere in den kubernetes/ Ordner und wende die Konfigurationen an:  kubectl apply -f .

3. Zugriff auf die App
Prüfe die laufenden Services:  kubectl get svc

Dieses Projekt wurde zu Lernzwecken erstellt, um die Brücke zwischen Softwareentwicklung (Dev) und IT-Betrieb (Ops) zu schlagen.
