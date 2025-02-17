# Deep Reinforcement Learning para Design de Peptídeos Antimicrobianos

## Descrição do Projeto
Este projeto utiliza técnicas de Deep Reinforcement Learning (DRL) para projetar novos peptídeos antimicrobianos, visando combater a resistência antimicrobiana. 

## Objetivos
### Objetivo Geral
Este trabalho, tem como objetivo utilizar ferramentas \acf{drl} para \emph{design} de \acf{pam} para futuramente serem validados \emph{in vitro}.

### Objetivos específicos
Este trabalho contém como objetivos específicos:
- Explorar e consolidar conhecimento sobre peptídeos antimicrobianos (PAMs) e suas propriedades estruturais e funcionais para subsidiar a geração computacional de novos compostos.
- Investigar a aplicabilidade de técnicas de deep reinforcement learning (DRL) no design de PAMs, avaliando seus benefícios e limitações no contexto da descoberta de novos peptídeos bioativos.
- Contribuir para o avanço de estratégias computacionais para descoberta de biomoléculas ao propor um modelo baseado em DRL capaz de sugerir novos (PAMs) com potencial terapêutico.
- Fornecer um conjunto de peptídeos candidatos que poderão ser futuramente validados experimentalmente, gerando insights para pesquisas futuras no desenvolvimento de novos antimicrobianos.

## Estrutura do Repositório
- `dados/`: Contém os dados que foram selecionados, atualizados, e filtrados para serem usados no modelo.
- `codigo/`: Códigos-fonte do treinamento dos modelos. A mesma metodologia foi usada, por isso ambor apresentam extrema similaridade.
- `resultados/`: Os resultados obtidos pelo modelo.
  - `resultados/modelo/`: Gráficos gerados durante o treinamento que mostram a efetividade dos peptídeos, e os dados dos 50 peptídeos com maior recompensa selecionados para análise in silico.
  - `resultados/peptideos_gerados/`: Consiste dos 50 peptídeos obtidos pelo modelo e selecionados em formato .fasta.
  - `resultados/brutos/`: Contém os testes realizados sobre os peptídeos sem houver limpeza detalhada. Inclui as características dos peptídeos, as predições de toxicidade e hemólise, e as predições de atividade antimicrobiana pelos várias ferramentas descritas no trabalho.
  - `resultados/processados/`: Contém os testes que passaram por uma limpeza e agrupamento para uso na apresentação do trabalho. São esses os testes de toxicidade e hemólise (hemotox), e as predições de atividade antimicrobiana (amp_predic).
  - `resultados/principais_peptidos/`: Contém os dados acerca dos 6 melhores peptídeos gerados. Isso inclui a predição de cada uma das ferramentas, e a média de sucesso dos peptídeos, e as figuras das representações de suas estruturas pela ferramenta HeliQuest.
