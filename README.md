#### Template para rodar o Vue.js com Tauri

Tauri é uma ferramenta similar ao Electron, para gerar aplicativos multiplataformas  
Roda no compilador do Rust

Vue.js + Quasar
Vite + Tauri

Este template possui os seguintes recursos configurados
- [x] Vue.js 3.0 com todos os seus recursos
- [x] Quasar UI // suporte a todos os componentes do [quasar](https://quasar.dev/)
- [x] [Vite](https://vitejs.dev/) 
- [x] i18n // suporte para traduções
- [x] axios // permite fazer requisições http
- [x] routes // permite configurar rotas, múltiplas plastas
- [x] componentes  
- [x] pinia // permite configurar um store global
- [x] Biblioteca de ícones

![](dashboard.PNG)

# Pré-requisitos

Conheça as tecnologias deste template  
https://vitejs.dev/   
https://vuejs.org/  
https://quasar.dev/   
https://tauri.app/  

Se você tem interesse em Design acesse o guia Material Design  
https://m3.material.io/

Conheça a linguagem Rust  
rust-lang.org/pt-BR/

## É importante ter o ambiente configurado com as seguintes tecnologias
```shell
# https://nodejs.org/pt-br/ # node > 14
npm install --global yarn # yarn
yarn global add @vue/cli # vue cli
yarn global add @quasar/cli # quasar cli
```

## Rust  
Este projeto utiliza Tauri, que é uma biblioteca Rust para empacotar este projeto no formato .executável multiplataformas

Se você não pretende distribuir binários no formato .exe similares ao electron pode ignorar esta parte

Instale o Rust 
rust-lang.org/pt-BR/tools/install

Em seguida instale o Tauri
```shell
cargo install create-tauri-app
```

# Configurando Tauri

Este projeto foi criado com o comando `cargo create-tauri-app` ou similar `yarn create tauri-app`

# 
Para criar o seu próprio setup com vite
```shell
 yarn create vite
 # supondo que o projeto chama lab
 cd lab/
 yarn create tauri-app
 
```
# Clonando este repositório
```shell
git clone https://github.com/ricardodarocha/vite-quasar-tauri-template.git
yarn # para instalar as dependências
```

## Como rodar esta aplicação
```bash
yarn 
quasar dev
```

## Para construir a aplicação Java Script


```bash
quasar build
```

## Para construir os binários da aplicação tauri

```
cargo build 
cargo build --release
cargo run
```
![](mainlayout.PNG)
![](cadastromenu.PNG)
![](tabela.PNG)
