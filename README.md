# BancoImobiliario
Jogo do Banco Imobiliário

Considere o seguinte jogo hipotético muito semelhante a Banco Imobiliário, onde várias de suas mecânicasforam simplificadas. Numa partida desse jogo, os jogadores se alteram em rodadas, numa ordem definidaaleatoriamente no começo da partida. Os jogadores sempre começam uma partida com saldo de 300 paracada um.Nesse jogo, o tabuleiro é composto por 20 propriedades em sequência. Cada propriedade tem um custo devenda, um valor de aluguel, um proprietário caso já estejam compradas, e seguem uma determinada ordem notabuleiro. Não é possível construir hotéis e nenhuma outra melhoria sobre as propriedades do tabuleiro, porsimplicidade do problema.No começo da sua vez, o jogador joga um dado equiprovável de 6 faces que determina quantas espaços notabuleiro o jogador vai andar.Ao cair em uma propriedade sem proprietário, o jogador pode escolher entre comprar ou não apropriedade. Esse é a única forma pela qual uma propriedade pode ser comprada.Ao cair em uma propriedade que tem proprietário, ele deve pagar ao proprietário o valor do aluguel dapropriedade.Ao completar uma volta no tabuleiro, o jogador ganha 100 de saldo.Jogadores só podem comprar propriedades caso ela não tenha dono e o jogador tenha o dinheiro da venda.Ao comprar uma propriedade, o jogador perde o dinheiro e ganha a posse da propriedade.Cada um dos jogadores tem uma implementação de comportamento diferente, que dita as ações que elesvão tomar ao longo do jogo. Mais detalhes sobre o comportamento serão explicados mais à frente.Um jogador que fica com saldo negativo perde o jogo, e não joga mais. Perde suas propriedades e portantopodem ser compradas por qualquer outro jogador.Termina quando restar somente um jogador com saldo positivo, a qualquer momento da partida. Esse jogadoré declarado o vencedor.Desejamos rodar uma simulação para decidir qual a melhor estratégia. Para isso, idealizamos uma partidacom 4 diferentes tipos de possíveis jogadores. Os comportamentos definidos são:O jogador um é impulsivo;O jogador dois é exigente;O jogador três é cauteloso;O jogador quatro é aleatório;

O jogador 
impulsivo
 compra qualquer propriedade sobre a qual ele parar.
O jogador 
exigente
 compra qualquer propriedade, desde que o valor do aluguel dela seja maior do que 50.
O jogador 
cauteloso
 compra qualquer propriedade desde que ele tenha uma reserva de 80 saldo sobrando
depois de realizada a compra.
O jogador 
aleatório
 compra a propriedade que ele parar em cima com probabilidade de 50%.
