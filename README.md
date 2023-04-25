<p align="center">
  <img src="https://user-images.githubusercontent.com/60453269/234305382-af9af980-18e4-42ee-888c-b50f794c328a.png" alt="Logo" width="200" height="200" />
</p>


<h1 align="center"> Sistema de turmas </h1>

<a id="Sumário"></a>


<p align="center">
  <b> Api de um sitema de turmas </br>
  <sub> Um sistema desenvolvido para fins de estudos no backend e TypeSript </b>
  <sub>
</p>

[![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)](#table-of-contents)

<p align="center">
  <a href="#Introdução"> 🧩 Introdução </a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#Resultados"> 🚀 Resultados</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#Dependências"> 🧪 Dependências</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#Ideias">💡 Possíveis Melhorias </a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#Creditos"> 🏆 Créditos </a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</p>

<br/>
<br/>

🚧 Essa api não esta mais funcionando no heroko. Quando o projeto foi feito o heroko ainda era gratuito. Como o projeto é muito simples, basico e na epoca foi para fins de estudos optei por não  hospedar em outra plataforma gratuita, mas caso queira testar e usar é só seguir os passos te instalação.


<br/>


<a id="Introdução"></a>
## 🧩 Introdução 

  ***⠀⠀⠀⠀A api tem como finalidade gerenciar produtos em um banco de dados, tem 4 rotas principais, GET, POST, PUT, DELETE ou seja um crud. De modo geral 
  o projeto é bem simples, no GET é possível ver todos os produtos cadastrados, no POST tem como finalidade o cadastro de produto, além disso, 
  pode-se mudar alguns dados através do PUT, como nome do produto, preço entre outros. Já o DELETE como o próprio nome diz ele deleta os dados de
  todo o produto através do seu id.***

<br/>

<a id="Resultados"></a>
## 🚀 Resultados 
  > Todos os resultados foram alcançados com sucesso. De modo geral são esses os resultados de cada requisição. 

<br/> 
  
### 🎯 PEGAR TURMAS
  
### ```GET``` 
```URL

https://labenu-system-9.herokuapp.com/turmas
 
```
  
```JSON
  {
{
"nome":"Aluno",
"email":"Aluno@gmail.com",
"data_nasc":"02/02/2022",
"turma_id":"1662651616681"
},...
  }
```
  
<br /> 

### 🎯 Pegar Docentes
  
### ```GET``` 
```URL

https://labenu-system-9.herokuapp.com/docentes
 
```
  
```JSON
  {
{
"nome":"Bruno",
"email":"Bruno@gmail.com",
"data_nasc":"01/01/2000",
"turma_id":"1662651616681"
},...
  }
```
  
<br /> 
  
### 🎯  Add Turma
  
### ```POST```  
  
```URL
https://labenu-system-9.herokuapp.com/turmas

```
  
```JSON
{
  "nome":"Freire"
}
```

<br /> 

### 🎯  Add Docentes
  
### ```POST```  
  
```URL
https://labenu-system-9.herokuapp.com/docentes

```
  
```JSON
{
  "nome":"Bruno",
  "email":"Bruno@gmail.com",
  "data_nasc":"01/01/2000",
  "turma_id":"1662651616681"
}
```

<br /> 
  
### 🎯  Mudar Turma

  
### ```PUT```  
  
```URL
  https://labenu-system-9.herokuapp.com/turmas/turma
```
  
```JSON
{
  "id":"1662651616681",
  "modulo":"6"
}

```

<br/> 
  
### 🎯  Mudar Docente

  
### ```PUT```  
  
```URL
https://labenu-system-9.herokuapp.com/docente
```
  
```JSON
{
  "id_turma":"1662666336896",
  "id": "1662741262439"
}

```


<br/>

<a href="#Sumário"> 📖 Volta ao Sumário </a>

<br /> 

<a id="Dependências"></a>
## 🧪 Dependências
> Requisitos para rotar o codigo...
  
<br /> 


## `📖 Instalação` 


<br /> 

> Caso tenha Git basta da git clone, caso não tenha basta clicar em code e depois dowloand zip e seguir os proximos passos

```BASH
git clone https://github.com/MayconCoutinho/Sistema-de-Turma
```

<br /> 

> Caso já tenha o Node em sua maquina basta instalar o projeto com npm i

```BASH
npm i 
```
<br /> 

> OBS - Muito importante, caso não tenha um banco de dados MySQL disponivel, não vai da para rodar o projeto, pois o projeto conecta diretamente com o banco de dados
> sendo assim crie um arquivo ".env" para por os dados do MySQL.


```BASH

DB_HOST = Dados MySQL
DB_USER = Dados MySQL
DB_PASSWORD = Dados MySQL
DB_SCHEMA = Dados MySQL

```

<br /> 


## `📖 Scripts` 


```JSON
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "tsc && node ./build/index.js",
    "dev": "ts-node-dev ./src/index.ts",
    "migrations": "tsnd ./src/data/migration.ts"
  }
```

<br /> 


## `📖 Dependencies` 

```JSON
  "dependencies": {
        "@types/knex": "^0.16.1",
        "cors": "^2.8.5",
        "dotenv": "^16.0.2",
        "express": "^4.18.1",
        "knex": "^2.3.0",
        "mysql": "^2.18.1"
      }

```

<br /> 

## `📖 devDependencies` 


```JSON
      "devDependencies": {
        "@types/cors": "^2.8.12",
        "@types/express": "^4.17.13",
        "ts-node-dev": "^2.0.0",
        "typescript": "^4.8.2"
      }

```



<br /> 

<a id="Ideias"></a>
## 💡 Possíveis Melhoras
> Possíveis melhorias no código e no projeto, caso queira voltar e melhorá lo.

<br /> 

- [ ] ***- *** 



<br/>

<a href="#Sumário"> 📖 Volta ao Sumário </a>

<br /> 

<a id="Creditos"></a>
## 🏆 Créditos

<br /> 

<div align="center"> 

| [<img src="https://user-images.githubusercontent.com/60453269/217899761-dc2d4e4b-3336-419d-9076-79304290aa0a.png" width=200><br><sub> Maycon Coutinho </sub>](https://www.linkedin.com/in/maycon-coutinho/) |[<img src="https://user-images.githubusercontent.com/60453269/234314654-e2bbb31c-55fb-43c1-9abc-9651893643ca.png" width=200><br><sub> Marcia de Paula Mello </sub>](https://www.linkedin.com/in/maycon-coutinho/)|[<img src="https://user-images.githubusercontent.com/60453269/234314927-59dce824-b59b-4a9a-a46a-7aab60b443b9.png" width=200><br><sub>Leonardo Almeida </sub>](https://www.linkedin.com/in/maycon-coutinho/)  
|---|---|---|
 


</div> 

<br /> 


