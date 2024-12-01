# Projeto Games

## Visão Geral
Este é um projeto simples para aprendizado de novos conceitos e relembrar alguns pontos importantes sobre requisições HTTP, API, segurança de dados, boas práticas de programação web e acesso a dados.

No **front-end**, utilizamos **HTML puro** e **JavaScript** com **Axios** para requisições. No **back-end (API)**, usamos **JavaScript** com **Node.js** e bibliotecas como **Express**, **jsonwebtoken** e **body-parser**.

Foi utilizado neste projeto o **Node.js 20**.

---

## Conceitos

### **CRUD**
- Implementação dos conceitos de CRUD (*Create, Read, Update e Delete*) consumindo uma API para gerenciar dados de jogos.

### **HTTP**
- Utilização do Axios para facilitar as requisições HTTP e integrar o front-end com a API.

### **Tratamento de dados**
- Como tratar os dados antes de enviar em uma requisição HTTP e processar esses dados no back-end.

### **Rotas**
- Estruturação de rotas de envio e recebimento de dados, além da definição dos dados esperados em cada rota.

### **Segurança**
- Uso de **JWT (JSON Web Token)** para garantir segurança no envio e recebimento de dados sensíveis.

### **Interpretação de mensagens**
- Processamento do corpo das mensagens HTTP utilizando **body-parser**.

### **LocalStorage**
- Armazenamento de informações de acesso nos navegadores, além de como inserir e acessar esses dados.

---

## Aplicação

### Front-end
- **Tecnologias**: Desenvolvido em **HTML5** e **JavaScript** sem o uso de CSS. 
- Arquivo principal: **`index.html`** (localizado na pasta **`Consumo_API`**).
- Propósito: Foco no aprendizado de requisições e integração entre front-end e API.
- **Detalhes do código**:
  - O código **HTML** e **JavaScript** estão no mesmo arquivo.
  - A biblioteca **Axios** é incluída via **CDN**, adicionada no final do arquivo, antes da tag `</body>`.
  - Todas as funções e requisições (CRUD), bem como o tratamento de dados, estão encapsulados dentro da tag `<script></script>`.

### Back-end
- **Tecnologias**: Desenvolvido em **Node.js** com **Express**.
- Arquivo principal: **`index.js`**.
- Propósito: API básica e educacional, com toda a lógica implementada em um único arquivo.
- **Bibliotecas utilizadas**:
  - **body-parser**: Para interpretar o corpo das mensagens HTTP.
  - **jsonwebtoken**: Para criar tokens de autenticação.
  - **cors**: Para configurar políticas de acesso à API.
  - **express**: Para criar e gerenciar rotas e middlewares.
- **Mock de dados**: Os dados consumidos pela API estão definidos diretamente no arquivo.

---

## Instalação dos Recursos

Alguns recursos precisam ser instalados localmente caso você clone o repositório e deseje testar a aplicação, já que arquivos desnecessários para produção foram removidos para otimizar o tamanho do repositório.

### Pré-requisitos

#### **Node.js**
- Caso não tenha o **Node.js** instalado:
  - Baixe diretamente pelo site oficial: [https://nodejs.org/pt](https://nodejs.org/pt).
  - Ou use o **NVM (Node Version Manager)** para instalar e gerenciar múltiplas versões:
    - Instale o **NVM**: [NVM para Windows](https://github.com/coreybutler/nvm-windows).

#### **Node Modules**
- Para rodar o servidor, instale os módulos necessários na pasta **APIDeGames**:
```bash
    npm install
```

### Dependências do Projeto
Instale as bibliotecas a seguir:
#### **body-parser**
- Necessário para interpretar o conteúdo do corpo das requisições HTTP:
```bash
    npm install --save body-parser
```
#### **cors**
- Para configurar políticas de acesso da API:
```bash
    npm install --save cors
```
#### **jsonwebtoken**
Para criar tokens de autenticação:
```bash
    npm install --save jsonwebtoken
```


## Executando o servidor
Após instalar o Node.js e as dependências, execute o seguinte comando na pasta do projeto:
```bash
    node index.js
```

O servidor estará rodando e pronto para uso.

