# usp_ari
Repo para o codigo de ML utilizado no tcc de data science

A ferramenta utilizada para a construção é o MatLab, usando a metodologia transfer learning. O algoritmo usa uma rede neural já iniciada, chamada googlenet, que contém cerca de 22 camadas de profundidade, 7 milhões de parâmetros, e aceita imagens de tamanho 224-by224, conforme a documentação. Esta rede entra como fornecedora de informações básicas como modelagem de entrada, tamanho, quantidade de canais, etc.

A forma como transcorre o treinamento, é basicamente fazendo a substituição das últimas camadas de aprendizagem por camadas novas que estarão no final, e gerando uma nova camada de output (output layer), que usará os novos argumentos de imagens (a nova base de teste) para efetuar o treinamento do algoritmo.

Em seguida, entramos com os cálculos de acurácia, validação e predição do modelo, necessários para cálculo dos índices de qualidade da nossa base de treinamento.
