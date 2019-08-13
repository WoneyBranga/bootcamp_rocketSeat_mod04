Treinamento BootCamp RocketSeat - Módulo 03 - Introdução ao REACT
---

# 01 - Conceitos do React 

- React é uma biblioteca para construção de interfaces;
- React trabalha com conceito SPA *Single page application*;
- É uma Lib mas pode-se chamar de framework;
- No React TUDO fica dentro do Javascript;

Tipos do REACT:
- React - lib;
- React JS - comportamento do react no Browser;
- React Native - comportamento do react no celular;

## Vantagens do React

- organização do código
  - componetização;
- Divisão de responsabilidades;
 - back-end: regra de negocio;
 - front-end: interface;
- Uma API,  Múltiplos clientes;
- Programação Declarativa;

## JSX
- permite escrever html dentro do js;
-  com react podemos criar nossos proprios elementos;

## imperativo vs Declarativo

### Exemplo Imperativo
```jsx
const notificacoes = 0;
function montaBadge(num) {
 if (notificacoes === 0 && num > 0) {
  // Adiciona badge
  // container.appendChild(badge)!!.
 }

 if (notificacoes !== 0 && num > 0) {
  // Apenas muda o número
  // badge.innerHTML = num!!.
 }

 if (notificacoes !== 0 && num === 0) {
  // Remove badge
  // container.removeChild(badge)
 }
}
```

### Exempo Declarativo
```jsx
// Não comparamos com o estado anterior
function Badge({ num }) {
  return (
    <div id="container">
      { num > 0 && <div id="badge">{num}</div>}
      <span class="icon"></span>
    </div>
  );
}
```

## Babel / Webpack

- Browser nao entende codigo react;
- **Babel** Converte nosso código js de forma que browser entenda;
- Webpack:
  - criacao do bundle, aruivo com todo codigo da aplicacao;
  - Ensina ao js como importar arquivos css, imagens, etc;
  - Live reload com webpack dev server;

---

# 02 - configurando estrutura

```bash
yarn init -y
yarn add @babel/core @babel/preset-env @babel/preset-react webpack webpack-cli -D
yarn add react react-dom

yarn add babel-loader -D

yarn add webpack-dev-server -D
```

---

# 03 - Criando componente Raiz

---

# 04 - Importando CSS

```bash
yarn add style-loader css-loader -D
```

# 05 - Importando Imagens

```bash
yarn add file-loader -D
```
