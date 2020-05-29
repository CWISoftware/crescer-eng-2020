# Crescer 2020 - Engenharia

## Jogo da Forca
O objetivo desse desafio é desenvolver o Jogo da Forca em times de até 12 pessoas. 

### Especificação
Criar o Jogo da Forca, onde um usuário vai entrar na página do jogo e na páginal inicial será exibido o rank dos jogadores com mais pontos. Em cada linha do ranking exbirá o ID do jogada, nome do usuário, palavra, número de tentativas e a data da jogada.
Para um usuário jogar, ele clica no botão jogar que está na tela inicial. Nesse momento o sistema deverá selecionar uma palavra aleatória de um banco de palavras com no mínimo 50 palavras. Para cada letra da palavra será exibido na página da jogada um caracter '_' que representa da cada letra.
>**Exemplo**: Cachorro, deverá exibir _ _ _ _ _ _ _ _ _

O usuário deverá entrar uma letra. Se ela corresponder a alguma letra da palavra então deverá substituir o caracter '_' pela letra correspondente.
>**Exemplo**: Cachorro, _ _ _ _ _ _ _ _ _, usuário entra 'R', então exibir _ _ _ _ _ rr _

Se não corresponder a nenhum letra, então deve incrementar o numero de erros em 1. Quando o número de erros for igual a 7 então o usuário perdeu a jogada. A palavra correta deverá ser exibida.

O usuário inicia uma jogada com 7 pontos e cada vez que ele erra uma jogada, ou seja, a letra entrada não corresponde a nenhuma letra da palavra, então a pontuação da jogada é decrementada em 1. 
>**Exemplo**: Cachorro, _ _ _ _ _ _ _ _ _, usuário entra 'R', então exibir _ _ _ _ _ rr _. Usuário entra a letra B, então exibi _ _ _ _ _ rr _ e reduz a pontuação de 7 para 6.

A aplicação deverá enviar a cada 30 segundos as informações atualizadas do ranking para a API de Ranking, disponível abaixo em material de apoio. As informações que devem ser enviadas são ID da jogada, nome do jogador, palavra da jogada, número de tentativas, Timestamp da jogada. Essa API retornará um GUID confirmando que os dados foram recebidos. A aplicação deverá guardar essa informação.

## Material de apoio

- Músicas gratuítas: https://github.com/tannerhelland/free-music
- URL da API de Ranking: http://localhost
- Banco de imagens: https://unsplash.com/