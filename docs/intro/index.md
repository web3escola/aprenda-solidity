# Introdução ao Solidity

**Solidity** é a linguagem mais utilizada para se escrever contratos inteligentes. Ela foi desenvolvida para compilar para a máquina virtual da Ethereum (**EVM**, **E**thereum **V**irtual **M**achine), que está presente não apenas na rede Ethereum, porém em tantas outras redes, como a Polygon, BNB chain e Avalanche. Qualquer rede que seja compatível com a EVM pode ter contratos inteligentes escritos em Solidity.


Solidity é uma linguagem de alto nível, estaticamente tipada, que incorpora diversas características de uma linguagem de programação orientada a objetos, como herança, sobreposição de métodos, entre outros. Veremos tudo isso até o fim deste livro. 

Contratos inteligentes são como pequenos programas capazes de modificar estados na Ethereum. Estados são informações (em geral, criadas por variáveis definidas em contratos inteligentes) armazenadas na blockchain. Por exemplo, o saldo em ether (ou a moeda base da rede em questão) de uma determinada conta é um estado da rede. Em termos gerais, a EVM é uma máquina que altera estados através de transações. 

A principal característica da Ethereum é que ela é uma rede descentralizada. Seu estado global (world state) encontra-se replicado em diversos computadores (clientes/servidores) ao redor do mundo, que chamamos de **nós**. O que garante que todos os nós mantêm o mesmo exato estado global é o mecanismo de consenso da blockchain. Em termos mais técnicos, blockchains são um sistema distribuído.

O fato da Ethereum ser uma rede descentralizada, peer-to-peer, faz com que as aplicações que desenvolvemos para ela sejam chamados de aplicações descentralizadas, ou dApps. Aplicações descentralizadas em geral são formadas por um contrato inteligente e uma interface com o usuário, que se conecta com o contrato inteligente através de uma carteira. Veremos sobre carteiras em breve. 

Esse livro é sobre Solidity e a EVM. Ensinaremos a criar contratos inteligentes para a EVM, ou seja, contratos inteligentes que podem ser executados em qualquer blockchain que implemente uma EVM. Ao longo do caminho, iremos entender melhor o que é o estado global da rede, como transações modificam tais estados e, principalmente, como definir estados e transações em contratos inteligentes.

Além de Solidity, há outras linguagens que também compilam para a EVM, como Vyper, ainda que Solidity seja de longe a mais utilizada. Tanto Solidity quando Vyper são linguagens de alto nível, o que quer dizer que não é possível interagir diretamente com a memória, por exemplo.

Além de linguagens de alto nível, há também linguagens de baixo nível. A mais famosa delas chama-se **Yul** e pode ser utilizada tanto por si só, quanto juntamente com Solidity. Yul é como o Assembly da EVM e veremos sobre ele nos capítulos mais avançados.

Por fim, há o bytecode, que é o código que a EVM executa. Solidity, Vyper e Yul compilam para o bytecode, assim como qualquer outra linguagem que venha a ser desenvolvida para a EVM. Nenhum programador escreve diretamente em bytecode, ainda que seja tecnicamente possível. Ao fim deste livro, você entenderá a EVM a ponto de entender não apenas Solidity, como o bytecode.