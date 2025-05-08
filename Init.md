# Configurando o ambiente

## Command line tools

Baixe as ferramentas de desenvolvimento em linha de comando por: https://developer.android.com/studio, elas devem estar no final da página. Você deve escolher a opção Linux

Extraia o arquivo e renomeie para: "android-sdk", abra a pasta, abra a pasta "cmdline-tools" e crie uma nova pasta chamada: "latest". Mova todos os arquivos da pasta para a nova pasta

Abra a pasta: "latest", abra a pasta: "bin" com o terminal. Digite: "./sdkmanager "platform-tools"", após concluído o download, digite: "./sdkmanager "platforms;android-30"", após isso, digite: "./sdkmanager "build-tools;30.0.3""

Copie o caminho da pasta: "android-sdk" e digite: "nano ~/.bashrc", vá até o final e digite: "export ANDROID_HOME=*Caminho da pasta "android-sdk"*", salve o arquivo com Ctrl + S e feche o arquivo com Ctrl + X. Ainda no terminal, digite: "source ~/.bashrc"

## Java

Instale o Java com: "sudo apt install openjdk-17-jdk" e "sudo apt install openjdk-17-jre"

## SDK Man

Instale o SDKMan em https://sdkman.io/install

Que lhe instrui a digitar os seguintes comandos: "curl -s "https://get.sdkman.io" | bash", e logo após: "source "$HOME/.sdkman/bin/sdkman-init.sh""

## Gradle

Instale o Gradle com o seguinte comando: "sdk install gradle 7.5"

# Criando a aplicação

Crie uma nova pasta com o nome do seu aplicativo e abra esta pasta no terminal, digite: "gradle init", ele irá lhe fazer perguntas sobre qual tecnologia você usará no seu projeto

Clone a pasta: "ProgramStructure" como seu programa android e faça suas modificações

# Compilando

No terminal, vá para a raiz do seu projeto e digite: "./gradlew assembleDebug"

Seu APK deve estar em: app/build/outputs/apk/debug