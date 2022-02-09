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

## Comandos

### Instalação

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

### Coverage

Gerar relatórios:

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
