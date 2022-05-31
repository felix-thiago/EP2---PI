Exercício realizado por: 

Kauê Sales
Vynicius Zanardi
Gabriel Kenji
Thiago Félix

Representação do espaço de estados - Qual o tamanho N ideal da sua população? Outros valores melhoram ou pioram?
Função de Fitness: O quão próximo do ideal você está, aplicado a este caso, garantir que as vans percorram aproximadamente a mesma distância.
Função de Seleção: Sugestão aplicar a Seleção por tragédia depois de 1000 gerações:
Função de Mutação - Testar mais de um tipo de mutação. Qual é a taxa ideal de mutação? Outros valores melhoram ou pioram?
Função de Cross-Over - Qual é a taxa ideal de cross-over? Outros valores melhoram ou pioram?

Abaixo temos resultados de testes realizados que respondem e justificam os pontos acima.

Comparações de tamanho da população
Tamanho da População = 1000

:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[0, 10, 4, 2, 15, 0], [0, 4, 16, 3, 10, 0], [2, 15, 0, 0, 14, 12], [0, 15, 7, 16, 1, 0]]

Distância percorrida: 17276

Resultados: Van 1

Distância percorrida pela van 1 : 4860

Van 2

Distância percorrida pela van 2 : 4952

Van 3

Distância percorrida pela van 3 : 3332

Van 4

Distância percorrida pela van 4 : 4132

Distância percorrida Total (4 vans): 17276

Tamanho da População = 100
:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[0, 2, 15, 6, 3, 0], [10, 15, 0, 0, 2, 3], [5, 15, 0, 0, 2, 11], [0, 3, 14, 1, 16, 0]]

Distância percorrida: 17504

Resultados:

Van 1

Distância percorrida pela van 1 : 5180

Van 2

Distância percorrida pela van 2 : 3696

Van 3

Distância percorrida pela van 3 : 3880

Van 4

Distância percorrida pela van 4 : 4748

Distância percorrida Total (4 vans): 17504

Tamanho da População = 10
:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[0, 15, 2, 16, 3, 0], [10, 3, 0, 0, 15, 5], [6, 4, 0, 0, 2, 12], [14, 1, 0, 0, 11, 16]]

Distância percorrida: 15086

Resultados:

Van 1

Distância percorrida pela van 1 : 5136

Van 2

Distância percorrida pela van 2 : 3754

Van 3

Distância percorrida pela van 3 : 3286

Van 4

Distância percorrida pela van 4 : 2910

Distância percorrida Total (4 vans): 15086

Considerações: Analisando os resultados do cenário com tamanho de população igual a 1000, não temos uma mudança significativa comparado ao cenário com tamanho de 100, porém temos uma queda brusca de performance. E analisando o cenário com o tamanho de 10, temos uma melhora de performance mas os resultados foram piores se comparados aos outros cenários, que acabou sobrecarregando uma das vans, provando-se um cenário que não apresenta uma boa homogeneidade.

Teste Geração 100K
hiperparâmetros

tamanho_populacao = 100

tx_mutacao = 0.1

tx_crossover = 0.15

tx_tragedia = 0.05

geracoes_max = 100_000

geracoes_tragedia = 100

:::::::::::::::::::::::::::::::::::::::::::::: GEN: 100000 ::::::::::::::::::::::::::::::::::::::::::::::

[[0, 2, 11, 8, 15, 0], [0, 8, 11, 2, 15, 0], [14, 3, 0, 0, 2, 7], [0, 15, 6, 11, 4, 0]]

Van 1

Distância percorrida pela van 1 : 4724

Van 2

Distância percorrida pela van 2 : 4724

Van 3

Distância percorrida pela van 3 : 3446

Van 4

Distância percorrida pela van 4 : 4040

Distância percorrida: 16934

Teste Geração 10K
hiperparâmetros

tamanho_populacao = 100

tx_mutacao = 0.1

tx_crossover = 0.15

tx_tragedia = 0.05

geracoes_max = 10_000

geracoes_tragedia = 100

:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[0, 16, 4, 2, 15, 0], [3, 5, 0, 0, 15, 2], [0, 2, 13, 4, 10, 0], [0, 2, 11, 8, 15, 0]]

Van 1

Distância percorrida pela van 1 : 5112

Van 2

Distância percorrida pela van 2 : 3252

Van 3

Distância percorrida pela van 3 : 4268

Van 4

Distância percorrida pela van 4 : 4724

Distância percorrida: 17356

Considerações:

Realizamos testes com o número de gerações em 10.000 e 100.000 e identificamos que a diferença da distância percorrida pelas vans não foi tão significativa, levando em consideração o tempo de processamento dos dados. Portanto, chegamos à conclusão que é melhor manter um número reduzido de maximo de gerações para otimizar os testes.

População sem tragédia
:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[0, 15, 10, 9, 3, 0], [0, 2, 7, 6, 14, 0], [0, 15, 2, 5, 4, 0], [0, 1, 10, 6, 12, 0]]

Distância percorrida: 14172

Resultados: Van 1

Distância percorrida pela van 1 : 3856

Van 2

Distância percorrida pela van 2 : 3104

Van 3

Distância percorrida pela van 3 : 3948

Van 4

Distância percorrida pela van 4 : 3264

Distância percorrida Total (4 vans): 14172

População com tragédia
:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[0, 16, 4, 15, 2, 0], [8, 15, 0, 0, 3, 14], [0, 4, 16, 2, 13, 0], [3, 16, 0, 0, 15, 2]]

Distância percorrida: 17040

Resultados:

Van 1

Distância percorrida pela van 1 : 4908

Van 2

Distância percorrida pela van 2 : 3720

Van 3

Distância percorrida pela van 3 : 4064

Van 4

Distância percorrida pela van 4 : 4348

Distância percorrida Total (4 vans): 17040

Considerações:

De acordo com os resultados que possuem a condição de seleção com tragédia após 1000 gerações temos uma melhora na questão de eficiência, pois as vans percorrem um trajeto maior, mantendo uma diferença entre elas semelhante ao cenário sem tragédia.

Análise de Taxa de Mutação
hiperparâmetros tamanho_populacao = 100

tx_mutacao = 0.2

tx_crossover = 0.15

tx_tragedia = 0.05

geracoes_max = 10_000

geracoes_tragedia = 100

:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[6, 15, 0, 0, 3, 9], [0, 15, 6, 13, 2, 0], [0, 4, 13, 6, 15, 0], [0, 16, 3, 10, 4, 0]]

Distância percorrida: 17608

Resultados: Van 1

Distância percorrida pela van 1 : 3640

Van 2

Distância percorrida pela van 2 : 4816

Van 3

Distância percorrida pela van 3 : 4200

Van 4

Distância percorrida pela van 4 : 4952

Distância percorrida Total (4 vans): 17608

hiperparâmetros tamanho_populacao = 100

tx_mutacao = 0.1

tx_crossover = 0.15

tx_tragedia = 0.05

geracoes_max = 10_000

geracoes_tragedia = 100

:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[15, 2, 0, 0, 1, 10], [10, 1, 0, 0, 2, 15], [0, 11, 6, 1, 16, 0], [4, 16, 0, 0, 15, 6]]

Distância percorrida: 15988

Resultados:

Van 1

Distância percorrida pela van 1 : 3960

Van 2

Distância percorrida pela van 2 : 3960

Van 3

Distância percorrida pela van 3 : 4108

Van 4

Distância percorrida pela van 4 : 3960

Distância percorrida Total (4 vans): 15988

hiperparâmetros tamanho_populacao = 100

tx_mutacao = 0.01

tx_crossover = 0.15

tx_tragedia = 0.05

geracoes_max = 10_000

geracoes_tragedia = 100

:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[6, 11, 0, 0, 2, 15], [0, 2, 11, 16, 1, 0], [10, 13, 0, 0, 2, 15], [10, 4, 0, 0, 16, 3]]

Distância percorrida: 15622

Resultados:

Van 1

Distância percorrida pela van 1 : 3834

Van 2

Distância percorrida pela van 2 : 4656

Van 3

Distância percorrida pela van 3 : 3412

Van 4

Distância percorrida pela van 4 : 3720

Distância percorrida Total (4 vans): 15622

Considerações: Comparando os dois primeiros cenários com as taxas de mutação 0.2 e 0.1, podemos ver que ao reduzir a taxa de mutação tivemos um resultado próximo do ideal (fitness) onde a distância percorrida pelas vans foram quase todas idênticas. Olhando para o cenário onde a taxa de mutação foi 0.01, observa-se que o resultado já não foi tão agradavel, concluindo que reduzir a taxa de mutação trouxe melhores resultados porém até certo ponto.

Análise de Taxa de Cross Over
hiperparâmetros

tamanho_populacao = 100

tx_mutacao = 0.1

tx_crossover = 0.1

tx_tragedia = 0.05

geracoes_max = 10_000

geracoes_tragedia = 100

:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[11, 10, 0, 0, 15, 2], [4, 14, 0, 0, 2, 11], [0, 2, 4, 16, 3, 0], [2, 15, 0, 0, 16, 11]]

Distância percorrida: 16100

Resultados:

Van 1

Distância percorrida pela van 1 : 3742

Van 2

Distância percorrida pela van 2 : 3572

Van 3

Distância percorrida pela van 3 : 4952

Van 4

Distância percorrida pela van 4 : 3834

Distância percorrida Total (4 vans): 16100

hiperparâmetros

tamanho_populacao = 100

tx_mutacao = 0.1

tx_crossover = 0.5

tx_tragedia = 0.05

geracoes_max = 10_000

geracoes_tragedia = 100

:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[0, 8, 15, 11, 2, 0], [9, 1, 0, 0, 2, 15], [0, 16, 3, 2, 4, 0], [0, 3, 1, 2, 15, 0]]

Distância percorrida: 15826

Resultados: Van 1 Distância percorrida pela van 1 : 3720

Van 2 Distância percorrida pela van 2 : 3618

Van 3 Distância percorrida pela van 3 : 4472

Van 4 Distância percorrida pela van 4 : 4016

Distância percorrida Total (4 vans): 15826

hiperparâmetros

tamanho_populacao = 100

tx_mutacao = 0.1

tx_crossover = 0.01

tx_tragedia = 0.05

geracoes_max = 10_000

geracoes_tragedia = 100

:::::::::::::::::::::::::::::::::::::::::::::: GEN: 10000 ::::::::::::::::::::::::::::::::::::::::::::::

[[0, 14, 4, 8, 1, 0], [0, 9, 13, 6, 11, 0], [0, 2, 12, 5, 15, 0], [0, 10, 7, 3, 16, 0]]

Distância percorrida: 14652

Resultados:

Van 1

Distância percorrida pela van 1 : 3492

Van 2

Distância percorrida pela van 2 : 2944

Van 3

Distância percorrida pela van 3 : 4428

Van 4

Distância percorrida pela van 4 : 3788

Distância percorrida Total (4 vans): 14652

Considerações: analisando os cenários onde alteramos a taxa de crossover, não tivemos tanta mudança na parte de resultado, porém no cenário com a taxa de crossover 0.5 tivemos uma queda significativa de perfomance, logo podemos concluir que aumentar a taxa de crossover não é benéfico. E olhando para o cenário com a taxa de crossover 0.01, nota-se que se perdeu o equilibrio das distancias percorridas das vans, portanto diminuir muito a taxa se mostrou prejudicial.
