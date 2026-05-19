# ToggleMaster Auth Service

Microsserviço responsável pela autenticação da plataforma ToggleMaster.

## Responsabilidades

- Login
- Geração de token JWT
- Validação de autenticação
- Controle de sessão

## Stack

- Golang
- Docker
- Kubernetes
- GitHub Actions
- Amazon ECR
- Amazon EKS

## Execução local

```bash
go run cmd/main.go
Endpoint de Health Check
GET /health
Docker

Build:

docker build -t togglemaster-auth .

Run:

docker run -p 8080:8080 togglemaster-auth
CI/CD

Pipeline DevSecOps com:

Build
Unit Tests
GolangCI-Lint
Gosec
Trivy
Docker Build
Push para Amazon ECR
Deploy

Deploy automatizado via GitOps utilizando ArgoCD.



