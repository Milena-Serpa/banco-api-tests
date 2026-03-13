# Banco API Tests 🚀

Este projeto é uma suíte de automação de testes para a camada de API do projeto **[banco-api](https://github.com/juliodelimas/banco-api)**. Ele foi desenvolvido utilizando **JavaScript** para validar as principais funcionalidades, contribuindo para garantia da integridade das regras de negócio.

## 🛠️ Stack Utilizada

O projeto utiliza as seguintes tecnologias e bibliotecas:

* **Linguagem:** [JavaScript (Node.js)](https://nodejs.org/)
* **Framework de Testes:** [Mocha](https://mochajs.org/)
* **Biblioteca de Requisições:** [Supertest](https://github.com/ladjs/supertest)
* **Biblioteca de Asserções:** [Chai](https://www.chaijs.com/)
* **Gerenciamento de Ambiente:** [Dotenv](https://www.npmjs.com/package/dotenv)
* **Relatórios de testes:** [Mochawesome](https://www.npmjs.com/package/mochawesome)

---

## 📁 Estrutura de Diretórios

Abaixo está a organização das pastas e dos arquivos principais do projeto:

```text
├── tests/              
│   ├── login.test.js           # Testes de autenticação de usuários
│   └── transferencias.test.js  # Testes de fluxos de transferências bancárias
├── node_modules/       # Dependências e bibliotecas instaladas
├── .env                # Variáveis de ambiente (Ex: BASE_URL)
├── .gitignore          # Arquivos ignorados pelo sistema de versão
├── package.json        # Configurações, dependências e scripts do Node.js
└── mochawesome-report/ # Relatórios HTML gerados após a execução dos testes
```

## ⚙️ Configuração do Ambiente

Este projeto utiliza variáveis de ambiente para gerenciar a URL base da API. Isso permite que os testes sejam executados em diferentes ambientes sem alterar o código.

Para rodar os testes, crie um arquivo chamado **`.env`** na raiz do projeto e adicione a seguinte variável:

`BASE_URL=http://localhost:3000`

Substitua `http://localhost:3000` pela URL onde a API `banco-api` está rodando.
> **Atenção:** O arquivo `.env` contém informações de configuração local e não deve ser enviado para o repositório remoto.

---

## 🚀 Como Executar os Testes

Siga os passos abaixo para configurar e rodar os testes em seu ambiente:

### 1. Instalar as dependências
Certifique-se de que o Node.js está instalado e execute:
```text
npm install
```
### 2. Executar os testes
Para iniciar a execução de toda a suíte de testes:
```text
npm test
```

### 3. Obtenção de Relatórios
Após a execução, o **Mochawesome** gera um relatório visual detalhado. Você pode encontrá-lo em:
`./mochawesome-report/mochawesome.html`

---

## 🔗 Documentação das Dependências

* [Mocha Documentation](https://mochajs.org/)
* [Supertest GitHub](https://github.com/ladjs/supertest)
* [Chai Assertion Library](https://www.chaijs.com/api/bdd/)
* [Mochawesome Reporter](https://www.npmjs.com/package/mochawesome)
* [dotenv](https://www.npmjs.com/package/dotenv)
