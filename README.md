# Detector de mão

## Descrição 

Repositório criado para resolver o desafio de desenvolver um serviço que rode no navegador para detecção de mão, com o principal objetivo de predizer o ângulo theta, entre os pontos 8 e 4(imagem abaixo), em tempo real. O serviço foi criado utilizando Javascript/Typescript e teve como base a aplicação demo [Handpose](https://github.com/tensorflow/tfjs-models/tree/master/handpose)

## Pré-requisitos

* Instalar [MediaPipe](https://google.github.io/mediapipe/getting_started/install.html)

## Build

Entre na pasta:

```sh
cd Detector
```

Instale as dependências e prepare o diretório:

```sh
yarn
```
Para observar as alterações nos arquivos e iniciar um servidor:

```sh
yarn watch
```

Abra o servidor na porta indicada, Exemplo:
```http://localhost:1234
```

## If you are developing handpose locally, and want to test the changes in the demos

Cd into the handpose folder:
```sh
cd handpose
```

Install dependencies:
```sh
yarn
```

Publish handpose locally:
```sh
yarn build && yarn yalc publish
```

Cd into the demos and install dependencies:

```sh
cd demos
yarn
```

Link the local handpose to the demos:
```sh
yarn yalc link @tensorflow-models/handpose
```

Start the dev demo server:
```sh
yarn watch
```

To get future updates from the handpose source code:
```
# cd up into the handpose directory
cd ../
yarn build && yarn yalc push
```

