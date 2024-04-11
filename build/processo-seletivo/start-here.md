# :bell: INICIE AQUI
# 📑 Build Projeto - Processo Seletivo

Esta documentação é referente as etapas para o build do edu-lyc-processo-seletivo. Vamos seguir explicando o build do projeto para a versão 10.x que já suporta JAVA 11 e Tomcat 9. Caso seja necessário realizar com versões anteriores, certifique-se com sua liderança qual versão de JAVA e Tomcat deve ser utilizada.

## ⚙️Tecnologias

 - JAVA 11
 - GIT
 - Linux
 - Maven
 - Tomcat

### Preparando os diretórios dos projetos

O projeto **edu-lyc-processo-seletivo** depende do projeto **edu-lyc-api-soap** para funcionar. Portanto você vai precisar ter os dois projeto na sua máquina, porém em pastas separadas para poder executá-los simultaneamente em dois workspaces distintos no Eclipse.

Sugiro que sejam criados duas pastas com as seguintes estruturas:

- ~/github/lyceum-api-soap/develop
- ~/github/lyceum-processo-seletivo/develop

Criado esses dois diretórios na sua máquina, siga para o proximo documento: [Preparando edu-lyc-api-soap](./prepare-api-soap.md)
