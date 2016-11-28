# GeneraisBizatinosRelatorio
Relatório do trabalho dos Generais Bizantinos - FEI - CC7261 - Sistemas Distribuídos  

## Conceito
O problema dos Generais Bizantinos foi formulado por Lamport em 1981. Ele tem como objetivo estudar e propor uma solução para o problema de consenso em sistemas distribuídos, considerando que um sistema distribuído é composto por vários componentes conectados se comunicando por mensagens entre si existe a possibilidade de que algum, ou vários, destes nós falhem ou até mesmo comem a agir contra o objetivo do sistema. A ideia do algoritmo é estabelecer uma forma em que o sistema continue operando corretamente apesar das falhas individuais que possam ocorrer, garantindo portanto a propriedade de resiliência em um sistema distribuído.<br>
Para ilustrar o problema Lamport utilizou o exemplo de generais bizantinos planejando invadir uma vila, para que eles decidam sobre um plano de ação é necessário que haja comunicação entre eles por meio de mensagens, e considerando que pode haver generais traidores que irão tentar sabotar a comunicação é necessário estabelecer um esquema no qual a maioria dos generais honestos decidam por um mesmo plano de ação independente da tentativa de sabotagem dos traidores.<br>
Existem vários tipos de solução para este problema, dentre elas há a possibilidade de se utilizar assinaturas digitais para atestar que as mensagens recebidas foram realmente originadas por quem as proclama e que não foram alteradas no meio do caminho. Desta forma os generais podem manter um histórico confiável de ordens e de quem as originou para portanto inferir um bom plano de ação.<br>
  
## Redução
O problema dos Generais Bizantinos pode ser “reduzido” ao problema de um general se comunicando com seus militares subordinados, o general envia ordens e os militares subordinados devem entrar em consenso sobre qual plano de ação tomar. O menor escopo deste problema consiste em um general e dois militares subordinados:

