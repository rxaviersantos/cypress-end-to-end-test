<h1 align="center"> Cypress End to End Testing </h1>

<p align="center">
Um exemplo simples de uso do Cypress para testes de ponta a ponta
</p>

<p align="center">
  <img alt="License" src="https://img.shields.io/badge/License-MIT-green.svg">
</p>

# O que é o teste de ponta a ponta

O teste de ponta a ponta ( comumente conhecido como E2E) é um tipo de método de teste no qual um aplicativo é testado do início ao final de um fluxo de teste. Esses fluxos são predefinidos de acordo com as funcionalidades/condições a serem verificadas para uma execução bem-sucedida desse aplicativo. Geralmente, os fluxos de ponta a ponta são baseado nas interações do usuário e em como eles executam várias ações no aplicativo. 



<p align="center">
  <img alt="https://www.freecodecamp.org/news/why-end-to-end-testing-is-important-for-your-team-cb7eb0ec1504/" src="https://github.com/rxaviersantos/cypress-end-to-end-test/assets/85380530/577dc23f-616b-4337-948e-642b48f73bb5">
</p>

Conforme indicado aqui, a pirâmide mostra de baixo para cima: Unidade, Integração, E2E. À medida que você sobe a pirâmide, os testes ficam mais lentos para escrever / executar e mais caros ( em termos de tempo e recursos ) para executar / manter. É para indicar que você deve gastar mais do seu tempo em testes de unidade devido a esses fatores. Uma coisa que não mostra é que enquanto você sobe a pirâmide, o o quociente de confiança de cada forma de teste aumenta. Você ganha mais dinheiro por seu dinheiro. Portanto, embora os testes E2E possam ser mais lentos e mais caros que os testes de unidade, eles trazem muito mais confiança de que seu aplicativo está funcionando pretendido.

## Iniciando novo repositório 
Dentro da pasta do projeto, crie uma nova pasta e abra o terminal ou prompt de comando, digite o comando abaixo: 
```bash 
npm init
```
Depois da instalação estiver concluída, insira o comando abaixo para instalar os pacotes de dependências. 
### Intalando os pacotes de dependências 
```bash 
npm install
```
Logo após instalar todas as dependências, insira o comando abaixo para instalar o Cypress.
```bash 
npm install cypress –-save-dev
```
O comando acima instalará o Cypress localmente como uma dependência de desenvolvimento para o seu projeto.

### Instalando o XPath Plugin usando o comando abaixo

 ```bash 
npm install cypress-xpath
```
Ao instalar o plugin ```cypress-xpath``` adicione a linha de código abaixo em ```support/e2e.js```

 ```js
require('cypress-xpath');
```

### Criando o arquivo .gitignore

 ```bash 
touch .gitignore
```
O arquivo .gitignore é um arquivo de texto que diz ao Git quais arquivos ou pastas ele deve ignorar em um projeto, dentro do arquivo iremos ignorar a pasta  ```node_modules```

### Abrindo o Cypress 
 ```bash 
npx cypress open
```

### Executando o Cypress via linha de comando em modo headless
 ```bash 
npx cypress run 
```
O comando acima irá executar todos os testes existentes na mesma pasta.
 ```bash 
npx cypress run --spec cypress/e2e/e2e.cy.js
```

O comando acima irá executar somente um arquivo específico.


Obs.: É recomendado criar ```npm scripts``` no arquivo ```package.json``` com atalhos para a execução de tais comandos. Veja o ```scripts``` abaixo.

````json
{
  "name": "end-to-end",
  "version": "1.0.0",
  "description": "Um exemplo simples de uso do Cypress para testes de ponta a ponta",
  "main": "index.js",
  "scripts": {
    "test": "cypress run"
  },
  "keywords": [
    "Cypress",
    "JavaScript"
  ],
  "author": "Rodrigo Xavier",
  "license": "ISC",
  "devDependencies": {
    "cypress": "^12.12.0",
    "cypress-xpath": "^2.0.1",
    "dependency-version-badge": "^1.11.0"
  }
}
```` 

## Screenshots

Executando o teste Cypress end to end  
<p align="center">
  <img alt="" "height="700px" width="1020px"> </p>

## Rodando localmente

Clone o projeto

```bash
  git clone https://link-para-o-projeto
```

Entre no diretório do projeto

```bash
  cd my-project
```

Instale as dependências

```bash
  npm install
```

Inicie o servidor

```bash
  npx cypress open
```

       

-------
<p align="center">
 Olá, sinta-se à vontade para mostrar apoio e dar a este repo<img src="https://img.icons8.com/fluency/20/null/star.png"/>estrela! Significa muito, obrigado :) 
</p>
