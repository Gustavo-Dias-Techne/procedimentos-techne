# 📑 Build Projeto - Lyceum

Esta documentação é referente as etapas para o build do edu-lyc-lyceum, levando em consideração que foi utilizado java 11, caso seja necessario utilizar em outras versões de java, apenas lembre-se de alterar a versão do console para java 8.
Apenas as branchs: Develop e support/10.0.x utilizam o Java 11. As demais branchs seguem o mesmo procedimento, utilizando o java 8.

## ⚙️Tecnologias

 - JAVA 11
 - GIT
 - Linux

## ▶️ Executando Projeto

Primeiramente clique nesse link e configure seu settings.xml para prosseguir:
[Configurar Settings.xml](https://dev.azure.com/technecloud/lyceum-ng/_wiki/wikis/lyceum-ng.wiki/567/Configurar-settings.xml-do-maven)

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
