# 📑 Build Projeto - Lyceum


## ⚙️Tecnologias

 - JAVA 11
 - GIT
 - Linux

## ▶️ Executando Projeto

Faça o clone do projeto edu-lyc-hades:
```
$ git clone git@github.com:technecloud/edu-lyc-hades.git
```
Após o clone, faça o checkout para a branch da develop:
```
$ git checkout develop
```
Execute o build do projeto utilizando o mvnw:
```
$ ./mvnw clean install -U
```
Após sucesso do build, navegue até a pasta raiz dos seus repositorios e faça o clone do edu-lyc-lyceum:
```
$ git clone git@github.com:technecloud/edu-lyc-lyceum.git
```
Faça o checkout para a branch da develop:
```
$ git checkout develop
```
Navegue até a pasta lyceum-dependecies
```
$ cd lyceum-dependencies
```
Execute o clean install:
```
$ ./mvnw clean install -U
```
Após sucesso, retorne para a raiz do edu-lyc-lyceum e execute o build:
```
$ cd ..
```
```
$ ./mvnw clean install -U
```
Pronto.
