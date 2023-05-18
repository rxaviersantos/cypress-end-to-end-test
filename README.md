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

## Iniciando projeto 

```bash 
npm init
```
