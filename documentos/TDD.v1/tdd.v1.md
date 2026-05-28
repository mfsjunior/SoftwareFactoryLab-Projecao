### 1. Tipos de comunicação (Backend ↔ Frontend)
- RESTful API (JSON)
**- **WebSockets (Socket.io)

### 2. Convenções de Nomenclatura
- **API/JSON:**  camelCase
- **Banco de Dados:** snake_case

### 3. Arquitetura de Integração
- **Microserviços:** 
  - Backend (negócio)
  - Inteligencia (IA/MediaPipe) 
  - Banco de Dados (Fornece os Dados)
  - Frontend (UI/UX, apresentacao)

### 4. Definição de contrato e esquema de dados
- **OpenAPI (Swagger)**

### 5. Estratégia de autenticação e autorização
- JWT (JSON Web Tokens)
- RBAC (Role-Based Access Control)

### 6. Tratamento de erros e padronização
- **Estrutura Global:** Retorne sempre um objeto padronizado em caso de erro:
    JSON
    { 
        "error": "TYPE_CODE", 
        "message": "Descrição amigável", 
        "timestamp": "...", 
        "details": {}        
    }

- **Códigos de Status HTTP:** 
  - 400 para erro de validação
  - 401 para non-authenticated
  - 403 para forbidden
  - 429 para timeout

### 7. Fluxo de trabalho (Dev & Implantação)
- **GitFlow**
- **CI/CD**: basicamente testes unitários
- **Docker**

### 8. Gerenciamento de estado e cache
- **Cache (Redis): **armazenamento de sessao por exemplo

### 9. Observabilidade e registro de logs
- Logs Centralizados
- Monitoramento

### 10. Dependências e ferramentas
- **Backend:** Spring Boot (Java 21+)
-** Servico:** FastAPI (Python 3.12+).
- **Frontend:** Next.js, Tailwind CSS, ShadcnUI.