# node-projetct-template
A template for node backend projects


## Configurando ambiente VSCODE

### Instalação de dependências para DEV

#### Curl 
    sudo apt install curl

#### NodeJS by NVM
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
    source ~/.bashrc
    nvm list-remote
    nvm install v1X.6.0
    nvm use v1X.6.0
    
#### NPM
    sudo apt install npm
    
#### Nodemon
    npm install nodemon   


### Extensões

#### Babel
npm install --save-dev babel-cli babel-preset-env
##### Configurar o arquivo package.json

    "start": "nodemon --exec babel-node src/app.js",
    "build": "rimraf dist && babel src/ -s -D -d dist ",
#### rimraf
##### Objetivo: habilitar a execução do comando rm -rf no Windows
##### Instalação npm install --save-dev babel-cli babel-preset-env
###### Criar arquivo  .babelrc na raiz do projeto com seguinte conteúdo:
{
  "presets": ["env"]
}

### Testes 
#### Instalando o JEST
npm install --save-dev jest

#### Usando JEST com Babel
Para usar Babel, instale as dependências necessárias via yarn:

yarn add --dev babel-jest @babel/core @babel/preset-env

###Dependências comuns a projetos de API e consulta a banco de dados


## Referências
#### -  https://blog.risingstack.com/10-best-practices-for-writing-node-js-rest-apis/
#### -  https://www.youtube.com/watch?v=joTc5o9lFCg
