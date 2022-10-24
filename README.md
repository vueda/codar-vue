## O que é o Vue?

É um framework/biblioteca JavaScript para construir interfaces de usuário (UI).

Seu foco é principalmente a criação de componentes utilizando HTML, CSS e JavaScript.

**Documentação:** https://vuejs.org/

**Recomendação de curso:**

- https://treinamento.vuejsbrasil.org/
- https://www.alura.com.br/formacao-vuejs3
- https://www.vuemastery.com/

## Criando um card com informações do GitHub

Vamos utilizar o Vue para criar um componente de card que exibe as informações de um usuário do GitHub.

<div style="text-align:center">
    <img src="./docs/github-card.png" width="250" />
</div>

## Preparação

- Instale o [NodeJS](https://nodejs.org/en/).
- Execute o seguinte comando para criar um novo projeto Vue:

        npm init vue@latest

- Responda as perguntas para a configuração do projeto.
- Siga as instruções após a criação do projeto.

Obs: O `NodeJS` é um ambiente de execução(runtime) JavaScript. Ele permite que você execute código JavaScript fora do navegador.

Junto com a sua instalação vem o `npm (Node Package Manager)` que é um gerenciador de pacotes, ou seja, ele permite que você instale diversas biblioteca e frameworks para utilizar no seu projeto.

## Estrutura do projeto

Ao criar o projeto você encontrará a seguinte estrutura:

```
.vscode                 -> Arquivos relacionados a IDE
node_modules            -> Todas as dependências do seu projeto ficam aqui
public                  -> Conteúdo estático que vai ser diretamente copiado para a sua pasta de distribuição final
src                     -> Código fonte do projeto
- assets                -> Conteúdo estático que vai ser tratado pela ferramenta de build
- components            -> Componentes que compõe a sua aplicação
- App.vue               -> Arquivo SFC (Single File Component) que representa a página inicial
- main.js               -> Entrypoint do projeto. É aqui que ocorre a inicialização, assim como a importação de dependências e outras configurações.
- .eslintrc.cjs         -> Configurações do linter (ESLint)
- .prettierrc.json      -> Configurações do formatador (Prettier)
- index.html            -> Arquivo inicial que importa o main.js. É a partir dele que
- package.json          -> Scripts e dependências do projeto
- package-lock.json     -> Representa a exata árvore de dependências instaladas. Não é alterado manualmente.
- vite.config.js        -> Configurações da ferramenta de build e servidor de desenvolvimento (Vite)
```

### O que são ESLint, Prettier e Vite

**ESLint**

Ferramenta para análise de código. Ela procura por potenciais problemas no seu código.

https://eslint.org/docs/latest/rules/

**Prettier**

Ferramenta para formatação de código.

https://prettier.io/docs/en/index.html

**Vite**

Ferramenta para build e servidor de desenvolvimento.

https://vitejs.dev/

## Info

background-color: #161b22

color: #8b949e

npm install --save @fortawesome/fontawesome-free

import '@fortawesome/fontawesome-free/css/all.css'

<span class="fas fa-location-dot"></span>

<span class="fas fa-building"></span>
