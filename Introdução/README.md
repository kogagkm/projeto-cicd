# Projeto: "Pipeline CI/CD Básico com Docker e GitHub Actions"

## Objetivo
Criar um pipeline CI/CD que automatize o build, teste e deployment de uma aplicação simples em Python (ou linguagem de sua escolha), utilizando Docker e GitHub Actions.

## Descrição do Projeto

### Aplicação Simples
Crie uma aplicação simples em Python (por exemplo, uma API básica com Flask ou FastAPI). A aplicação pode ter apenas um ou dois endpoints para simplificar, como um endpoint `GET /status` que retorna um JSON com uma mensagem de status.

### Configuração do Docker
- **Dockerfile**: Crie um arquivo Dockerfile para sua aplicação. Isso permitirá a criação de uma imagem Docker.
- **Docker Compose**: Crie um `docker-compose.yml` para definir um ambiente de desenvolvimento com a sua aplicação e, opcionalmente, um banco de dados (por exemplo, PostgreSQL ou MySQL).

### Teste da Aplicação
- Escreva testes unitários básicos para a aplicação usando uma biblioteca como `pytest`.
- Inclua um teste para o endpoint de status.

### Pipeline de CI/CD com GitHub Actions
- **CI (Continuous Integration)**: Configure um workflow no GitHub Actions para construir a aplicação (usando o Docker), executar os testes e fazer o push da imagem Docker para o Docker Hub (ou GitHub Container Registry).
- **CD (Continuous Deployment)**: Configure um segundo workflow para fazer deploy da aplicação em um servidor de staging ou produção (pode ser um servidor simples como uma VM na AWS, DigitalOcean ou um ambiente local usando Docker Compose).

### Documentação
Crie um `README.md` explicando os passos para reproduzir o projeto, incluindo instruções para rodar localmente, construir a imagem Docker e configurar o pipeline CI/CD.

## Tecnologias/Ferramentas Utilizadas
- **Linguagem de Programação**: Python
- **Ferramenta de Contêiner**: Docker
- **Orquestrador**: Docker Compose
- **Ferramenta de CI/CD**: GitHub Actions
- **Controle de Versão**: GitHub

## Passos Extras
Caso queira avançar, pode adicionar monitoramento com Prometheus e Grafana para monitorar o uso de recursos (CPU, memória, etc.) da aplicação Dockerizada.

## Resultado Esperado
O objetivo deste exercício é ganhar experiência prática configurando pipelines básicos, entender a automação com Docker e aprender a integrar testes no fluxo de desenvolvimento.
