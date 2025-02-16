Mega Man Robots API Documentation

Documentação gerada com auxílio de IA (ChatGPT, GitHub Copilot e Mermaid AI)
Índice

    Visão Geral

    Pré-requisitos

    Instalação

    Uso da API

    Endpoints

    Diagramas de Fluxo

    Contribuição

    Como a IA Foi Utilizada

Visão Geral

API para gerenciar robôs do universo de Mega Man, permitindo operações CRUD (Create, Read, Update, Delete). Desenvolvida em Python/Flask com integração a um banco de dados SQLite.

Recursos Principais:

    Listar todos os robôs.

    Buscar robô por ID.

    Adicionar/Remover/Atualizar robôs.

    Filtrar por tipo (Ex: "Maverick", "Boss").

Pré-requisitos

    Python 3.8+

    Flask

    SQLAlchemy

Instalação

Passos gerados com GitHub Copilot:

    Clone o repositório:
    bash
    Copy

    git clone https://github.com/seu-usuario/mega-man-robots-api.git  

    Instale as dependências:
    bash
    Copy

    pip install -r requirements.txt  

    Execute a aplicação:
    bash
    Copy

    python app.py  

Uso da API

Exemplos de requisições gerados pelo ChatGPT:
Listar todos os robôs:
bash
Copy

curl http://localhost:5000/api/robots  

Adicionar um robô:
bash
Copy

curl -X POST -H "Content-Type: application/json" -d '{"name": "Zero", "type": "Maverick", "weapon": "Z-Saber"}' http://localhost:5000/api/robots  

Endpoints

Tabela gerada com ChatGPT via prompt: "Crie uma tabela em markdown para endpoints CRUD"
Método	Endpoint	Descrição
GET	/api/robots	Lista todos os robôs
GET	/api/robots/<id>	Busca robô por ID
POST	/api/robots	Adiciona novo robô
PUT	/api/robots/<id>	Atualiza dados de um robô
DELETE	/api/robots/<id>	Remove um robô
Diagramas de Fluxo

Diagramas criados com Mermaid AI (ferramenta de IA para diagramação).
Fluxo de Requisição GET:
mermaid
Copy

sequenceDiagram  
    Client->>API: GET /api/robots  
    API->>Database: SELECT * FROM robots  
    Database-->>API: Dados dos robôs  
    API-->>Client: JSON Response (200 OK)  

Como a IA Foi Utilizada
Ferramenta	Uso	Exemplo de Prompt Utilizado
ChatGPT	Gerar exemplos de código e documentação	"Escreva um tutorial para endpoints REST"
GitHub Copilot	Autocompletar código e comentários	Sugerir docstrings para funções Flask
Mermaid AI	Criar diagramas de sequência	"Gere um diagrama para GET /api/robots"
Contribuição

    Faça um fork do projeto.

    Crie uma branch: git checkout -b feature/nova-funcionalidade.

    Envie as alterações: git push origin feature/nova-funcionalidade.

    Abra um Pull Request.

🔗 Repositório GitHub: mega-man-robots-api-docs
Resultado Final:

Captura de Tela da Documentação

Documentation powered by AI 🤖
Passos para Reproduzir:

    Substitua seu-usuario no GitHub pelo seu username.

    Adicione imagens na pasta assets/.

    Use o Mermaid Live Editor para ajustar diagramas.