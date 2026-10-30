# Simulador de Copa Universitária

Projeto final da disciplina de Lógica de Programação e Algoritmos, do 1º semestre de Engenharia de Software da UCSAL. Desenvolvido individualmente em Java.

## Sobre o projeto
Aplicação de console para gerenciar uma competição de futebol entre seleções universitárias. Durante a execução, o usuário cadastra as seleções e os jogadores, registra os resultados das partidas e consulta estatísticas da competição.

## Funcionalidades
- Cadastro de 5 seleções e de 11 jogadores para cada seleção.
- Busca de seleções e jogadores pelos nomes ou números de inscrição.
- Registro dos jogos de ida e volta entre todas as seleções.
- Consulta do campeão, dos artilheiros e do desempenho das seleções e dos jogadores.
- Cálculo de percentuais de jogadores que marcaram gols e de jogadores com mais de 5 gols.
- Ranking das seleções por pontos.

## Regras da competição
- Cada par de seleções se enfrenta duas vezes: uma partida de ida e outra de volta. Ao todo, são 20 partidas, e cada seleção disputa 8 jogos.
- Uma vitória vale 3 pontos; um empate vale 1 ponto para cada seleção.
- O campeão é definido pela maior pontuação. Em caso de empate, vence a seleção com mais gols marcados.
- O ranking é ordenado somente pela pontuação; em caso de empate, a ordem de cadastro é mantida.

## Tecnologias e conceitos
- Java e `Scanner` para entrada de dados pelo terminal.
- Vetores (`String[]` e `int[]`) e matrizes (`String[][]` e `int[][]`) para armazenar seleções, jogadores, pontos e gols.
- Estruturas condicionais (`switch` e `if`), repetição (`do-while` e `for`) e métodos para organizar as funcionalidades.

## Como rodar
Na raiz do projeto, compile e execute:

1. Compile o programa:
   ```bash
   javac src/Sistema_Copa_Universitaria.java
   ```
2. Execute:
   ```bash
   java -cp src Sistema_Copa_Universitaria
   ```

É necessário ter o JDK instalado. Os dados são mantidos apenas durante a execução e não são salvos em arquivo.

## Observações
- A opção de gol contra está disponível no registro da partida, mas esses gols não são contabilizados nas estatísticas de gols das seleções nem dos jogadores.
- Os menus esperam opções numéricas; gols e números de inscrição também devem ser informados como números.
