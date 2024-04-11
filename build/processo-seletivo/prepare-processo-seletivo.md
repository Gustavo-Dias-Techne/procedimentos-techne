## :zap: Preparando edu-lyc-processo-seletivo

Depois da preparação do projeto **edu-lyc-api-soap**, estamos prontos para realizar a subida do projeto **edu-lyc-processo-seletivo**.

##### 2.1 - Clone o projeto edu-lyc-processo-seletivo

Entre no repostório [edu-lyc-processo-seletivo](https://github.com/technecloud/edu-lyc-processo-seletivo) e faça o clone do projeto a partir da branch develop. Lembre-se de clonar esse projeto na pasta `~/github/lyceum-processo-seletivo/develop` citada anteriormente.

##### 2.2 - Execute o build do projeto usando o Maven

Dentro do terminal, vá até o diretório onde você realizou o clone do projeto e execute o comando:
```
./mvnw clean install -U
```
Caso ocorra o seguinte erro durante a execução do comando:
![image](https://github.com/Gustavo-Dias-Techne/procedimentos-techne/assets/144055556/f95532b0-ce6a-43c6-8b95-480c0c5e933b)\
Execute o comando abaixo e tente novamente:
```
chmod +x mvnw
```
Aguarde até que a build mostre a mensagem de sucesso. (*A primeira execução costuma demorar um pouco para ser completada*)

##### 2.3 - Abrindo o projeto no Eclipse

Abra seu eclipse, mas na seleção de *workspaces* lembre-se de selecionar a pasta `~/github/lyceum-processo-seletivo/develop`.

![image](./assets/processo-seletivo/eclipse-workspace-select.png)

Durante a primeira execução, seu workspace virá vazio, realize a importação do projeto acessando `File > Import Project` e selecionando a opção **Existing Maven Projects**.

![image](./assets/processo-seletivo/eclipse-import-project.png)
![image](./assets/api-soap/eclipse-import-project-select.png)
Logo após a importação, o Eclipse irá iniciar o processo de *build* do projeto. Aguarde até que a operação seja concluída. (Esta etapa pode demorar alguns minutos)

![image](./assets/api-soap/eclipse-import-project-build.png)

