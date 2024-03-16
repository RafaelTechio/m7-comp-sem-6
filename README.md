# Ponderada Semana 6 - Computação
Rafael Mateus Zimmer Techio

## Introdução

Ao resolver problemas do mundo real a partir de modelos de aprendizagem de máquina, é necessária atenção às mudanças que ocorrem em comportamentos de usuários, viéses e significados com o passar do tempo. Quando há uma mudança nesse sentido que impacta a acurácia do modelo, essa problemática é denominada "concept drift". Dessa forma, abordagens que solucionem ou diminuam os impactos das alterações de conceito são necessárias para engenheiros que utilizam recursos de aprendizagem de máquina para resolução de desafios reais.

## Solução Proposta

Como proposta de solução para a problemática de concept drift, a abordagem do paradigma de aprendizado contínuo é uma solução, contemplando os seguintes passos:

![image](https://github.com/RafaelTechio/m7-comp-sem-6/assets/110608373/9eb89f02-0c37-4eab-be3b-b2929bd38ee1)

Assim como todo modelo, é necessária a coleta de dados, pipeline de pré processamento a fim de transformar os dados em algo "entendível" para o algoritmo, o treinamento do modelo em si, alguns testes para a validação de seus resultados e o deploy para que possa ser implementado ou consultado por outros sistemas. Contudo, o paradigma de aprendizado contínuo adiciona uma etapa de testes automatizados periódicos, que podem ser realizados a partir de uma amostra atualizada de dados. Dessa forma, pode-se identificar uma queda na acurácia média do modelo em determinados cenários. Para resolver a questão, uma nova coleta de dados atualizada, com os conceitos corretos, é usada para reiniciar todo o processo de criação do modelo até o deploy de uma nova versão adaptada para o cenário real. Esse processo pode ser realizado automaticamente por meio de alertas como a diminuição das métricas de assertividade do modelo, em períodos de tempo ou até mesmo manualmente por algum administrador.

## Conclusão

Contudo, acredito ser inviável a implantação de modelos para a resolução de problemas sem uma estratégia de re-treino em algum momento. Sabe-se que o comportamento humano muda constamente e as variáveis de ambiente também, desse modo, pouquíssimas situações podem dispensar a abordagem de aprendizado contínuo e manterem-se com alta assertividade em seus contextos. Ainda que os gatilhos que disparem o fluxo de criação de uma nova versão do modelo possam ser complexos, é um esforço necessário para as situações que necessitam de soluções de IA, porém, o acionamento humano ainda pode auxiliar. Dessa forma, em ambos os casos, devem haver testes automatizados e que cubram grande parte das possibilidades de cenários possíveis, a fim de gerar métricas e identificar fenômenos como concept drift e outros.

## Referências Bibliográficas

BARBOZA, Eduardo Victor Lima; DE ALMEIDA, Paulo Ricardo Lisboa. Challenges on Classifying Data Streams with Concept Drift. In: WORKSHOP DE TESES E DISSERTAÇÕES (WTDBD) - SIMPÓSIO BRASILEIRO DE BANCO DE DADOS (SBBD), 37. , 2022, Búzios. Anais [...]. Porto Alegre: Sociedade Brasileira de Computação, 2022 . p. 126-132. DOI: https://doi.org/10.5753/sbbd_estendido.2022.21854.
