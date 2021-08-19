# Instalando ferramentas de desenvolvimento. 
Fala, galera! Hoje vim aqui trazer um tutorialzinho para quem, assim como eu, é usuário do Sistema Operacional Linux, mais precisamente da distribuição Ubuntu. Dito isso, seguiremos.

## Instalando o Andorid Studio 
A configuração do Android Studio pode ser feita com apenas alguns cliques.

Primeiro, verifique se você [fez o download da versão mais recente do Android Studio.](https://developer.android.com/studio/install?hl=pt-br#64bit-libs)

Para instalar o Android Studio no Linux, faça o seguinte:

1. Descompacte o arquivo `.zi` transferido por download em um local apropriado para seus aplicativos, como `/usr/local/` para seu perfil de usuário ou `/opt/` para usuários compartilhados.
Se você estiver usando uma versão de 64 bits do Linux, primeiro instale as bibliotecas necessárias para máquinas de 64 bits.

2. Para iniciar o Android Studio, abra um terminal, navegue até o diretório `android-studio/bin/` e execute `studio.sh`.
   
3. Selecione se você quer ou não importar as configurações anteriores do Android Studio e clique em **OK**.
4. O assistente de configuração do Android Studio orientará você durante o restante do processo, o que inclui o download dos componentes do SDK do Android que são necessários para o desenvolvimento.

### Bibliotecas necessárias para máquinas de 64 bits 
Se você estiver executando uma versão do Ubuntu de 64 bits, será necessário instalar algumas bibliotecas de 32 bits com o seguinte comando:

~~~
sudo apt-get install libc6:i386 libncurses5:i386 libstdc++6:i386 lib32z1 libbz2-1.0:i386
~~~

E é isso. Caso você tenha dificuldade, acesse [clique aqui](https://developer.android.com/studio/videos/studio-install-linux.mp4?hl=pt-br) para seguir todas as estapas do procedimento de configuração recomendado. 

## NodeJS
Nesta seção iremos instalar o nodeJs e o gerenciador de pacotes NPM (Node Package Manager). 
1. Abre o terminal (use as teclas Ctrl + Alt + T);
2. Atualize o gerenciador de pacotes e o sistema com o comando:
~~~
sudo apt update && sudo apt upgrade
~~~
3. Em seguida, instale o node.js dos repositórios oficiais com esse comando:
~~~
sudo apt install nodejs
~~~
4. Isso instalará o node.js. No entanto, em muitos casos, você precisa do gerenciador de pacotes NPM, que não é instalado por padrão com esse método. Para isso, use esse outro comando:
~~~
sudo apt install npm
~~~
5. Finalmente, após instalar o Nodejs no Ubuntu 20.04 e derivados, podemos consultar a versão instalada do node.js e nmp:
~~~
nodejs -v
~~~
~~~
npm -v
~~~
## React Native 
Para realizar a instalação do react-native ou react-native-cli, é importante que você tenha o NPM (Node Packager Manager) instalado na sua máquina, pois utilizaremos o gerenciador de pacotes do JavaScript para realizar a instalação. Caso você não tenha, siga o tópico anterior
1. Instalando o react-native utilizando o comando abaixo:
~~~
npm install react-native
~~~
2. Instalando o react-native-cli utilizando o comando abaixo:
~~~
npm install react-native-cli
~~~
3. Utilize o comando abaixo para verificar as versões que foram instaladas:
~~~
react-native --version
~~~
Deverá exibir a seguinte saída no terminal:****
![image](https://user-images.githubusercontent.com/71051791/130004352-e539fd15-12af-45ba-be5b-f81017628738.png)


