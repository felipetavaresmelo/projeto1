# Aprenda a testar Aplicações Javascript com Vedovelli

## Site da proposta do curso

https://javascript.tv.br

## Site das aulas

https://classes.vedovelli.com.br/

## Conteúdo

MÓDULO 1: INTRODUÇÃO AOS TESTES NO JAVASCRIPT

- Porque testar e o que testar
- Tipos de testes
  - Unitários
  - Integração
  - End to End (E2E)
  - Pirâmide de testes
- Como os testes garantem a integridade da aplicação
  - Github Actions
  - CI/CD
- Ferramentas
  - Jest
  - Cypress
- Libraries
  - Testing Library
  - Vue Test Utils
  - Enzyme
- Projeto 1 - Pequena Lib e uma classe
  - Criar projeto, instalar e configurar o Jest
  - Desenvolver com TDD uma lib para fazer parse de Query String
    -Desenvolver com TDD uma classe para gerenciar um carrinho de compras

## Notas

### [Instalação do Jest](https://jestjs.io/docs/getting-started)

Instalação no projeto como dependencia de desenvolvimento:

```sh
yarn add -D jest @types/jest
```

### Inicializar os testes

Inicializar para avaliar apenas uma vez.

```sh
yarn test
```

Inicializar para ficar monitorando os testes e recompilando a cada salvamento de arquivo.

```sh
yarn test:watch
```

### [Prettier](https://prettier.io)

Arquivo `.prettierrc.json` com configurações de formatação de código utilizada com essa extensão.

```sh
yarn add -D prettier
```

### Coverage

Gerar relatórios de cobertura de testes:

```sh
yarn test --coverage
```

Instalar o serviço para abrir os relatórios

```sh
sudo npm i -g httpserver
```

Navegar até a pasta do relatório e inicialisar o serviço do relatório de cobertura:

```sh
cd coverage/lcov-report
httpserver
```

Também pode abrir o index.html diretamente em um browser.

### [Babel](https://jestjs.io/docs/getting-started#using-babel)

Ferramenta utilizada compilar e resolver questões de compatibilidade de códigos TS modernos com versões antigas do JS.

```sh
yarn add --dev babel-jest @babel/core @babel/preset-env
```

### [Editor Config](https://editorconfig.org)

Arquivo `.editorconfig` utilizado para customizar formatação de código e uso de plugins já integrado em várias IDEs.
Utilzado aqui principalmente para configuração da quantidade de espaços em branco nas identações.

### [Lodash](https://lodash.com/docs/4.17.15)

Biblioteca de utilitários, utilizada aqui para find e remove na lista do Cart.

```sh
yarn add lodash
```

- [find](https://lodash.com/docs/4.17.15#find)
- [remove](https://lodash.com/docs/4.17.15#remove)
