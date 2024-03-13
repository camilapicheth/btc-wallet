<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="40px" src="https://hermes.digitalinnovation.one/assets/diome/logo-minimized.png"></a>
    <span> Criando e Utilizando uma Carteira de Criptomoedas</span>
</h1>


Repositório documentando um desafio de projeto **blockchain**: construir um gerador de carteiras bitcoin, importá-la para software específico e executar transações de envio e recebimento de bitcoin. 

   
## Objetivo 

Trabalhar com o desenvolvimento de um gerador de carteiras e realizar transações com bitcoin. Projeto realizado para o curso **"Formação Blockchain Specialist"**, da plataforma [Digital Innovation One](https://www.dio.me/), sob a orientação do professor Cassiano Peres. 


## Tecnologias 

[![JavaScript](https://img.shields.io/badge/JavaScript-000?style=for-the-badge&logo=javascript&logoColor=30A3DC)]() 
![Static Badge](https://img.shields.io/badge/Electrum%20Bitcoin%20Wallet%20-%20blue?logo=blockchain) 
![Static Badge](https://img.shields.io/badge/Bitcoin%20Faucet%20Generator%20-%20black?logo=bitcoin) 
<br>

## Projeto
<table>
  <thead>
    <tr align="left">
      <th>Nº</th>
      <th>Etapas</th>
    </tr>
  </thead>
  <tbody align="left">
    <tr>
      <td>01</td>
      <td>Desenvolvimento do Código no VS Code</td>
    </tr>
    <tr>
      <td>02</td>
      <td>Transição para o Electrum Bitcoin Wallet</td>
    </tr>
    <tr>
      <td>03</td>
      <td>Realizando Transações com Bitcoin de Teste</td>  
    </tr>
  </tbody>
  <tfoot></tfoot>
</table>

______________

## Etapa 1: Desenvolvimento do Código no VS Code 

O início do nosso projeto é marcado pela utilização do **VS Code**, um ambiente de desenvolvimento integrado, para a elaboração do código em **JavaScript**. Esta é a base do nosso gerador de carteiras Bitcoin. 

Para dar suporte ao nosso desenvolvimento, procedemos com o download de dependências essenciais: 

- **bip39**: Para a geração de seeds de carteiras, que são conjuntos de palavras usadas para recuperar ou criar carteiras. 

- **bip32**: Fornece funcionalidades necessárias para a geração de carteiras, incluindo a criação de carteiras HD (Hierarchical Deterministic) que permitem uma organização mais segura e sistemática das chaves. 

- **bitcoinjs-lib**: Uma biblioteca abrangente que facilita a manipulação de operações com Bitcoin, incluindo a criação de endereços e transações. 

Com estas ferramentas em mãos, seguimos uma série de etapas para construir o código gerador de carteiras: 

1. Importamos as dependências. 

2. Definimos a rede Bitcoin a ser utilizada. 

3. Estabelecemos a estrutura para carteiras HD. 

4. Geramos um mnemonic como seed. 

5. Criamos a raiz da carteira HD. 

6. Geramos uma conta com chaves privadas e públicas. 

7. Criamos o endereço Bitcoin. 

8. Exibimos os dados da carteira: endereço, chave privada e seed.

______________
 
## Etapa 2: Transição para o Electrum Bitcoin Wallet 

Para realizarmos as transações com Bitcoin de teste, escolhemos o **[Electrum Bitcoin Wallet](https://electrum.org/)** como nossa plataforma de transação. Após o download e instalação do software na máquina local, habilitamos o modo *testnet*, para simular transações sem o uso de bitcoins reais, proporcionando um ambiente seguro para testes. 

Com o Electrum pronto, procedemos à **importação da chave privada gerada anteriormente no VS Code**. Esta chave é o elo de ligação com a nossa carteira personalizada, agora apelidada de "dio-wallet-testnet" dentro do Electrum. Esse processo confere ao Electrum a capacidade de acessar e gerenciar os bitcoins de teste que nossa carteira irá movimentar.  

Assim, com a chave privada devidamente importada, nossa carteira no Electrum está operacional, pronta para iniciar o envio e recebimento de bitcoins de teste. 

______________

## Etapa 3: Realizando Transações com Bitcoin de Teste 

Com nossa carteira prontamente configurada no Electrum e a chave privada importada, avançamos para a etapa final do nosso projeto: a execução de transações de envio e recebimento de bitcoin na testnet. 

Para acompanhar as movimentações e validar as transações, utilizamos o **[Blockstream Explorer](https://blockstream.info/testnet/address/mmf6xDXxF9vCvqv99GJkWuJckM5bNt7Yue)**. Este explorador de blocos permite-nos visualizar detalhadamente o endereço da nossa carteira e as transações associadas a ela. 

Iniciamos o processo obtendo a quantia de 0.00039732 bitcoin de teste, recorrendo a um **Bitcoin Faucet**. Este recurso possibilita simular transações sem custo real, fornecendo bitcoins de teste que podem ser usados livremente na rede testnet. 

Para efetuar uma transação de envio, geramos um novo endereço através do nosso código no VS Code. Este novo endereço serve como destino para o valor total disponível em nossa carteira de teste. Ao concluir esta transação, não só validamos a funcionalidade do nosso gerador de carteiras como também testamos com sucesso a integração e operação dentro do ambiente de testnet do Bitcoin. 

______________

Desta forma, concluímos o desafio de projeto. Tínhamos como meta construir um gerador de carteiras bitcoin a partir do zero, importar essa carteira para um software especializado e, finalmente, executar transações de envio e recebimento de bitcoin na testnet. 
