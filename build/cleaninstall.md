# 📑 Build Projeto - Lyceum

Esta documentação é referente as etapas para o build do edu-lyc-lyceum, levando em consideração que foi utilizado java 11, caso seja necessario utilizar em outras versões de java, apenas lembre-se de alterar a versão do console para java 8.\
☕️ Apenas as branchs: Develop e support/10.0.x utilizam o Java 11. As demais branchs seguem o mesmo procedimento, utilizando o java 8.

## ⚙️Tecnologias

 - JAVA 11
 - GIT
 - Linux

## ▶️ Executando Projeto

Primeiramente clique nesse link e configure seu settings.xml para prosseguir:\
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
Caso ocorra esse erro ao executar o mvnw:\
![image](https://github.com/Gustavo-Dias-Techne/procedimentos-techne/assets/144055556/f95532b0-ce6a-43c6-8b95-480c0c5e933b)\
Execute o comando abaixo e tente novamente:
```
chmod +x mvnw
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
Após finalização, abra o eclipse, execute o maven update:
![image](https://github.com/Gustavo-Dias-Techne/procedimentos-techne/assets/144055556/dea4e1d8-9aab-47af-a533-6b3ef2222788)\
Selecione todos os projetos e clique em OK:\
![image](https://github.com/Gustavo-Dias-Techne/procedimentos-techne/assets/144055556/1835b1ed-945d-4961-be86-311e0c735d52)\
Para melhor desempenho do update, abra a aba progress e deixe apenas 1 update executando, clicando em parar nos demais, como na imagem abaixo:\
![image](https://github.com/Gustavo-Dias-Techne/procedimentos-techne/assets/144055556/34adaa3d-1f8f-4111-aab7-10f2bd45a08a)\
Assim, apenas um processo de update é executado por vez:\
![image](https://github.com/Gustavo-Dias-Techne/procedimentos-techne/assets/144055556/74ac9f65-1745-4967-a0ae-017d7ee462de)\
Após finalização do update, execute o Build All:\
![image](https://github.com/Gustavo-Dias-Techne/procedimentos-techne/assets/144055556/eef200fa-4755-4058-a692-092a78c26cf7)\
Na aba Servers, na parte inferior, execute o clean do Tomcat:\
![image](https://github.com/Gustavo-Dias-Techne/procedimentos-techne/assets/144055556/a458f071-6d9d-45e0-95c0-756dd1c6a310)\
Após isso, pode executar o debug 🪲.
