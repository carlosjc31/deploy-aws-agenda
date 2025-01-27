# 📅 Agenda de Compromissos

<div align="center">

![Badge Nome](https://img.shields.io/badge/Nome-Valor-cor)

![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)

</div>

Uma aplicação web completa para gerenciamento de compromissos, desenvolvida com Angular no frontend e Java Spring Boot no backend. O sistema permite que usuários gerenciem seus compromissos de forma eficiente e intuitiva.

## 🚀 Tecnologias Utilizadas

### Frontend
- Angular 16
- TypeScript
- Angular Material
- RxJS
- SCSS

### Backend
- Java 17
- Spring Boot 3
- Spring Security
- Spring Data JPA
- PostgreSQL
- Maven

### DevOps
- Docker
- Docker Compose
- AWS EC2
- Nginx

## 📋 Funcionalidades

- Autenticação e autorização de usuários
- CRUD completo de compromissos
- Filtros de busca por data, título e status
- Notificações de compromissos próximos
- Interface responsiva e moderna
- Persistência de dados em PostgreSQL
- Deploy automatizado na AWS

## 🛠️ Estrutura do Projeto

```
├── frontend/
│   ├── src/
│   ├── Dockerfile
│   └── package.json
├── backend/
│   ├── src/
│   ├── pom.xml
│   └── Dockerfile
├── docker-compose.yml
├── nginx/
│   └── nginx.conf
└── README.md
```

## 💻 Pré-requisitos

- Node.js 18+
- Java JDK 17
- Docker e Docker Compose
- Maven
- PostgreSQL (para desenvolvimento local)

## 🔧 Instalação e Execução Local

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/agenda-compromissos.git
cd agenda-compromissos
```

2. Configure as variáveis de ambiente:
```bash
cp .env.example .env
# Edite o arquivo .env com suas configurações
```

3. Execute com Docker Compose:
```bash
docker-compose up -d
```

A aplicação estará disponível em `http://localhost:80`

### Execução sem Docker

#### Backend
```bash
cd backend
mvn spring-boot:run
```

#### Frontend
```bash
cd frontend
npm install
ng serve
```

## 📦 Deploy na AWS

1. Crie uma instância EC2 na AWS
2. Configure as regras de segurança para as portas 80 e 443
3. Instale o Docker e Docker Compose na instância
4. Clone o repositório e configure as variáveis de ambiente
5. Execute o Docker Compose

```bash
docker-compose -f docker-compose.prod.yml up -d
```

## 🔒 Variáveis de Ambiente

```env
# Backend
SPRING_DATASOURCE_URL=jdbc:postgresql://db:5432/agenda
SPRING_DATASOURCE_USERNAME=postgres
SPRING_DATASOURCE_PASSWORD=senha
JWT_SECRET=your-secret-key

# Frontend
API_URL=http://localhost:8080/api
```

## 📚 Documentação da API

A documentação da API está disponível através do Swagger UI em:
`http://localhost:8080/swagger-ui.html`

## 🤝 Como Contribuir

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Faça commit das suas alterações (`git commit -m 'Add some AmazingFeature'`)
4. Faça push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## ✅ Testes

### Backend
```bash
mvn test
```

### Frontend
```bash
ng test
```

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Autor

LinkedIn: - https://www.linkedin.com/in/josé-carlos-carneiro/

## 🙏 Agradecimentos

- Agradeça aqui pessoas ou recursos que te ajudaram no desenvolvimento
