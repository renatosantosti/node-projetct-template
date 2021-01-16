# node-projetct-template
A template for node backend projects


## Configurando ambiente VSCODE
### Extensões

### Instalação de dependências para DEV
#### Nodemon
#### NVM
#### Babel
npm install --save-dev babel-cli babel-preset-env
##### Configurar o sarquivo package.json

    "start": "nodemon --exec babel-node src/app.js",
    "build": "rimraf dist && babel src/ -s -D -d dist ",
#### rimraf
##### Objetivo: habilitar a execução do comando rm -rf no Windows
##### Instalação npm install --save-dev babel-cli babel-preset-env
###### Criar arquivo  .babelrc na raiz do projeto com seguinte conteúdo:

{
  "presets": ["env"]
}

###Dependências comuns a projetos de API e consulta a banco de dados


## Referências
#### -  https://www.youtube.com/watch?v=joTc5o9lFCg
