# MyGroceryApp | Nickolas Bazar | Bazar do Nickolas | Teste de React Native - Aplicativo de Compras Online

Bem-vindo ao MyGroceryApp, um aplicativo de compras online desenvolvido com React Native. Este aplicativo permite que os usuários naveguem por uma variedade de produtos, adicionem itens ao carrinho, escolham métodos de pagamento e muito mais. Este guia o ajudará a configurar, executar e contribuir para o aplicativo. Certifique-se de seguir os passos com atenção para evitar problemas de configuração.

## Pré-requisitos

Antes de começar, verifique se você possui as seguintes ferramentas instaladas em sua máquina:

- *Node.js:* Certifique-se de ter o Node.js instalado na versão 14 ou superior. Você pode baixá-lo em [nodejs.org](https://nodejs.org/).

- *npm:* O npm geralmente é instalado junto com o Node.js. Verifique se ele está instalado executando `npm -v` no terminal.

- *React Native CLI:* Instale a CLI do React Native globalmente com o seguinte comando:

  bash
  npm install -g react-native-cli
  

- *Android Studio:* Se você planeja desenvolver para Android, instale o Android Studio. Certifique-se de configurar um emulador Android ou conectar um dispositivo físico. Você pode baixar o Android Studio em [developer.android.com/studio](https://developer.android.com/studio).

- *Xcode:* Se você planeja desenvolver para iOS, instale o Xcode e configure um simulador iOS ou conecte um dispositivo físico. O Xcode está disponível na App Store.


## Configuração

1. *Clone o Repositório:*
   Clone este repositório para a sua máquina local e navegue para o diretório do projeto:

   bash
   git clone https://github.com/seu-usuario/mygroceryapp.git
   cd mygroceryapp
   

2. *Instale as Dependências:*
   Instale as dependências do projeto usando o npm:

   bash
   npm install
   

3. *Configuração de Plataforma:*

   - *Para Android:* Abra o Android Studio, configure um emulador ou conecte um dispositivo físico via USB. Certifique-se de que o dispositivo esteja configurado corretamente e seja reconhecido pelo Android Studio.

   - *Para iOS:* Abra o projeto no Xcode e escolha um simulador iOS ou conecte um dispositivo iOS físico via USB. Verifique se o Xcode concluiu o processo de configuração inicial para a plataforma iOS.

4. *Inicie o Aplicativo:*

   - *Para Android:* Execute o comando abaixo para iniciar o aplicativo no emulador ou dispositivo Android conectado:

     bash
     npm run android
     

     Se você enfrentar problemas com o Gradle ou com as dependências do Android, tente executar:

     bash
     cd android
     ./gradlew clean
     cd ..
     npm run android
     

   - *Para iOS:* Execute o comando abaixo para iniciar o aplicativo no simulador ou dispositivo iOS conectado:

     bash
     npm run ios
     

     Se você enfrentar problemas relacionados ao Xcode, tente executar:

     bash
     rm -rf ios/build
     npm run ios
     

5. *Teste o Aplicativo:*
   Verifique se o aplicativo é exibido corretamente no emulador ou dispositivo. Navegue pelas telas, adicione produtos ao carrinho e teste as funcionalidades.

## Possíveis Problemas e Soluções

- *Problemas de Build do Android:*
  Se você enfrentar problemas relacionados ao Gradle ou às dependências do Android, tente limpar o cache e reconstruir:

  bash
  cd android
  ./gradlew clean
  cd ..
  npm run android
  

- *Problemas de Build do iOS:*
  Se ocorrerem problemas relacionados ao Xcode, limpe a pasta de build e reconstrua:

  bash
  rm -rf ios/build
  npm run ios
  

- *Problemas de Dependências:*
  Se ocorrerem problemas relacionados a dependências, exclua a pasta `node_modules` e o arquivo `package-lock.json`, em seguida, execute `npm install` novamente.

Certifique-se de verificar a documentação oficial do React Native, Android Studio e Xcode se encontrar problemas mais complexos.

Nota: Verifique sempre a integridade do arquivo metro.config.js qualquer problema nesse arquivo pode impedir o processo de testes do sistema.
     

## Funcionalidades Principais

- *Lista de Produtos:* Navegue por uma lista de produtos disponíveis para compra. Cada produto inclui uma imagem, nome, preço e descrição.

- *Carrinho de Compras:* Adicione produtos ao carrinho de compras e veja automaticamente o valor total atualizado.

- *Método de Pagamento:* Escolha entre diferentes métodos de pagamento para concluir sua compra.

- *Lista de Favoritos:* Marque produtos como favoritos para acesso rápido posteriormente.

- *Pesquisa por Produto:* Procure produtos específicos usando palavras-chave.

- *Notificações:* Receba notificações sobre ofertas especiais e atualizações do aplicativo.

- *Cadastro e Edição de Endereços:* Cadastre e gerencie endereços de entrega.

## Tecnologias Utilizadas

- *React Native:* Framework para desenvolvimento de aplicativos móveis multiplataforma.
- *Redux Toolkit:* Gerenciamento de estado global do aplicativo.
- *React Navigation:* Navegação entre telas.
- *Async Storage:* Armazenamento local para informações como favoritos e endereços.
- *React Native Firebase:* Integração com o Firebase para autenticação e armazenamento em nuvem.
- *Razorpay:* Integração para processamento de pagamentos.
- *Jest:* Framework de testes.
- *Eslint e Prettier:* Ferramentas para manter a consistência do código.

## Contribuição

Se desejar contribuir com o MyGroceryApp, siga as instruções detalhadas no README do repositório. Certifique-se de que suas alterações são testadas localmente antes de enviar uma solicitação de pull.
