# Ciclo de Estudos

Este projeto consiste em uma aplicação full stack simples para **gestão de estudos**, inspirada no vídeo do [Matemática em Evidência](https://discord.com/channels/1150108025340837908/1297990787690397779/1297996114196299881).  

A aplicação permite gerenciar ciclos de estudos, adicionar tarefas e acompanhar o progresso, proporcionando uma maneira eficiente de organizar seus estudos.

---

## Tecnologias Utilizadas

- **PHP**: Para o desenvolvimento do back-end e construção de APIs RESTful.  
- **React**: Para criar uma interface dinâmica e interativa no front-end.  
- **MySQL**: Banco de dados relacional para armazenar as informações dos ciclos de estudos.  
- **Apache**: Servidor web para hospedar o back-end.  
- **Docker**: Para facilitar a criação e o gerenciamento de containers.  
- **Tailwind CSS**: Para estilização rápida e consistente da interface.

---

## Estrutura de Diretórios

A estrutura do projeto é organizada para separar claramente as responsabilidades de cada tecnologia:

````
/project
│
├── /backend (PHP)
│   ├── /app
│   │   ├── /controllers       # Controladores que manipulam as requisições
│   │   ├── /models            # Modelos que representam e interagem com o banco de dados
│   │   ├── /views             # (Opcional) Arquivos de visualização para debug ou testes
│   │   └── /routes            # Definição das rotas e endpoints
│   ├── /config                # Configurações, como conexão ao banco de dados
│   └── /public                # Ponto de entrada da aplicação (index.php)
│       └── index.php
│
├── /frontend (React)
│   ├── /src
│   │   ├── /components        # Componentes reutilizáveis da interface
│   │   ├── /pages             # Páginas principais da aplicação
│   │   ├── /services          # Comunicação com APIs (REST)
│   │   └── index.js           # Arquivo principal de entrada do React
│   └── package.json           # Configurações e dependências do projeto React
│
├── /infra
│   ├── docker-compose.yml     # Configuração para orquestração de containers
│   ├── /nginx                 # Configuração do proxy reverso (se necessário)
│   └── outros arquivos        # Arquivos de infraestrutura
````
---

## Protótipo do Projeto

O protótipo inicial da interface está disponível no **Figma**:  
[Acessar Prototipo](https://www.figma.com/design/7UA1VlE9Tj1smV5faG2Llr/Ciclo-de-estudos?node-id=0-1&t=qQNDYW1WGafzPgMg-1)  

---

## Funcionalidades Principais

1. **Gerenciamento de Tarefas**:
   - Adicionar, editar e excluir tarefas relacionadas aos ciclos de estudo.  
2. **Visualização de Progresso**:
   - Acompanhar o progresso diário ou semanal de estudos.  
3. **Integração Dinâmica**:
   - Front-end conectado ao back-end via API RESTful, para atualizações em tempo real.

---

## Como Rodar o Projeto

### Pré-requisitos

- [Docker](https://www.docker.com/) instalado.  
- Ambiente configurado com Node.js para executar o front-end.

### Passos

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/ciclodeestudos.git
   cd ciclodeestudos
   ```

2. Configure o ambiente Docker:
   ```bash
   cd infra
   docker-compose up
   ```

3. Instale as dependências do front-end:
   ```bash
   cd frontend
   npm install
   npm start
   ```

4. Acesse no navegador:
   - Front-end: [http://localhost:3000](http://localhost:3000)  
   - Back-end: [http://localhost:8080](http://localhost:8080)  

---

## Contribuindo

Sinta-se à vontade para contribuir com este projeto! Para começar:  

1. Faça um fork do repositório.  
2. Crie um branch para sua feature ou correção:
   ```bash
   git checkout -b minha-feature
   ```  
3. Commit suas alterações:  
   ```bash
   git commit -m "Adiciona minha nova feature"
   ```  
4. Envie para o repositório remoto:  
   ```bash
   git push origin minha-feature
   ```  
5. Abra um pull request.  

---

## Licença

Este projeto é licenciado sob a [MIT License](LICENSE).

---

Se precisar de mais informações ou ajuda, entre em contato! 🚀  
