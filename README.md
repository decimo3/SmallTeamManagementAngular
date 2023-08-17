# AngularFrontEnd

Projeto para migração da tecnologia RazorPages do repositório

## Instalando do zero:

Através do template fornecido pelo `ng new` eu pude inferir as dependências básicas para a aplicação mínima em Angular, configurada parcialmente na mão.

Esse é um exercício para aprender o funcionamento do framework por dentro, mesmo antes de escrever código nele. Ainda não sei exatamente o que cada dependência faz, porém estou estudando a estrutura para aprender.

A estrutura de arquivos do template é complexa, então irei testando arquivo a arquivo e verificando 

## Dependências:

```bash
npm install --save-dev @angular/cli @angular-devkit/build-angular typescript ts-loader tslib zone.js @types/jasmine jasmine-core karma karma-chrome-launcher karma-coverage karma-jasmine karma-jasmine-html-reporter
npm install --save @angular/core @angular/common @angular/compiler @angular/compiler-cli @angular/router @angular/platform-browser @angular/platform-browser-dynamic rxjs 
```

* **@angular/cli:** pacote com todas as ferramentas para a criação da aplicação em Angular. Em destaque o comando `ng` usado para _scaffolding_.
* **@angular/core:** núcleo da biblioteca criação de componentes. ela contém a base para a criação de aplicativos Angular.
* **@angular/common:** bilbioteca de funcionalidades comuns utilizadas em aplicativos Angular.
* **@angular/compiler:** biblioteca responsável por compilar os templates e componentes do Angular em código JavaScript executável.
* **@angular-devkit:** pacote usado para gerenciar todo o fluxo de trabalho de desenvolvimento e construção de um projeto Angular.
* **@angular/platform-browser:** biblioteca responsável pela inicialização do aplicativo Angular no navegador e integração dos componentes Angular na árvore do DOM da página;
* **@angular/platform-browser-dynamic:** permite que você inicie um aplicativo Angular dinamicamente no navegador para carregamento assíncrono de módulos.
* **rxjs:** é uma biblioteca de programação *reativa* que oferece suporte a fluxos de dados assíncronos e manipulação de eventos. Isso é especialmente útil para gerenciar comunicação assíncrona, manipulação de eventos DOM e tratamento de solicitações HTTP.
* **typescript:** biblioteca que traz o transpilador e as ferramentas necessárias para trabalhar com a linguagem.

## Configuração:

### 1. Configuração inicial do Angular:

A configuração do Angular é realizada pelo arquivo `angular.json` que define um workspace Angular.

Ao iniciar qualquer comando `ng`, ele irá verificar primeiramente as configurações do projeto nesse arquivo.

```json
{
  /* minimal workplace configuration `angular.json` */
  "$schema": "./node_modules/@angular/cli/lib/config/schema.json",
  "version": 1,
  "newProjectRoot": "projects",
  "projects": {}
}
```

### 2. Configuração inicial do TypeScript:

A configuração do TypeScript é realizada pelo arquivo `tsconfig.json` que define as opções de compilação.

```json
{
  /* minimal typescript configuration file `tsconfig.json` */
  "compilerOptions": {
    "target": "ES2022",
    "module": "ESNext",
    "strict": true,
    "esModuleInterop": true,
    "moduleResolution": "node",
  }
}
```

### 3. Criação de uma aplicação Angular

Utilize o comando abaixo para criar a aplicação Angular dentro do workspace.

Esse comando irá gerar a estrutura básica de uma aplicação para iniciar

```bash
npx ng generate application <name>
```

### 4. Adicionando atalho para comandos

O comando `ng` serve para muitos propósitos, adicionar eles no `package.json` é uma boa prática.

```json
{
  /* shotcuts to most usage commands */
  "scripts": {
    "ng": "ng",
    "start": "ng serve",
    "build": "ng build",
    "watch": "ng build --watch --configuration development",
    "test": "ng test"
  }
}
```

## Referências:

* Descrições das bibliotecas usadas no projeto: [ChatGPT@3.5](https://chat.openai.com/share/ce50e174-1a46-4761-9a0f-b4d2b69a3a44)
