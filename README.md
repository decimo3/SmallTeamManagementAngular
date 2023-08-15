# AngularFrontEnd

Projeto para migração da tecnologia RazorPages do repositório

## Instalando do zero:

Através do template fornecido pelo `ng new` eu pude inferir as dependências básicas para a aplicação mínima em Angular, configurada parcialmente na mão.

Esse é um exercício para aprender o funcionamento do framework por dentro, mesmo antes de escrever código nele. Ainda não sei exatamente o que cada dependência faz, porém estou estudando a estrutura para aprender.

A estrutura de arquivos do template é complexa, então irei testando arquivo a arquivo e verificando 

## Dependências:

```bash
npm install --save-dev @angular/cli @angular-devkit/build-angular webpack webpack-cli webpack-dev-server typescript ts-loader
npm install --save @angular/core @angular/common @angular/compiler @angular/router @angular/platform-browser @angular/platform-browser-dynamic rxjs
```

* **@angular/cli:** 
* **@angular/core:** núcleo da biblioteca criação de componentes. ela contém a base para a criação de aplicativos Angular.
* **@angular/common:** bilbioteca de funcionalidades comuns utilizadas em aplicativos Angular.
* **@angular/compiler:** biblioteca responsável por compilar os templates e componentes do Angular em código JavaScript executável.
* **@angular-devkit/build-angular:**
* **@angular/platform-browser:** biblioteca responsável pela integração dos componentes Angular na árvore do DOM da página;
* **@angular/platform-browser-dynamic:** permite que você inicie um aplicativo Angular dinamicamente no navegador, em vez de iniciar em um ambiente pré-compilado. É usado quando você deseja criar aplicativos que são construídos e inicializados dinamicamente, como aplicações de renderização do lado do servidor (SSR) e carregamento assíncrono de módulos.
* **rxjs:** é uma biblioteca de programação *reativa* que oferece suporte a fluxos de dados assíncronos e manipulação de eventos. Isso é especialmente útil para gerenciar comunicação assíncrona, manipulação de eventos DOM e tratamento de solicitações HTTP.
* **webpack:** núcleo do gerenciador do webpack necessário para executar os pipelines configurados no arquivo `webpack.config.js`;
* **webpack-cli:** extensão do webpack que inicia via linha de comando a execução do pipeline configurado;
* **webpack-dev-server:** extensão do webpack que inicia o servidor de desenvolvimento que atualiza em tempo real o pipeline;
* **typescript:** biblioteca que traz o transpilador e as ferramentas necessárias para trabalhar com a linguagem.
* **ts-loader:** extensão do webpack que adiciona o typescript no pipeline do webpack; 

## Referências:

* Descrições das bibliotecas usadas no projeto: [ChatGPT@3.5](https://chat.openai.com/share/ce50e174-1a46-4761-9a0f-b4d2b69a3a44)
