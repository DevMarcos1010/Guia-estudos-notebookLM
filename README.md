# Ben, o notebookLM de investimentos

Ao explorar as capacidades do notebookLM e refletir sobre suas aplicações no cotidiano, surgiu a necessidade - e oportunidade - de iniciar um projeto que envolvesse uma dor minha. Um dos meus hobbies é nada mais do que operar uma pequena carteira de investimentos na B3, e uma dificuldade real do meu passatempo é fazer uma análise fundamental de ações, uma vez que no mercado mobiliário brasileiro existem centenas, até milhares de empresas, e encontrar a "melhor" é como tentar achar uma agulha no palheiro.

Para me ajudar com isso, criei um notebookLM que me ajudasse que essa tarefa, o [Ben](https://notebooklm.google.com/notebook/9479f68c-5c4b-485c-9bdc-edcf2e91634d) (para facilitar as referências) é um modelo de linguagem especialista em análise fundamentalista de ações. O objetivo deste notebookLM é auxiliar o investidor na filtragem de ações, seguindo metodologias bastante usadas no mercado, como as de Benjamin Graham, em "O investidor inteligente", e de outros autores renomados na área de investimentos como Peter Lynch e Mohnish Pabrai, além de influenciadores famosos como o Thiago Nigro, d'O Primo Rico, e Ramiro Gomes, do Clube do Valor. E além disso, com os ensinamentos destas personalidades e com acesso às notícias globais de economia, a gerenciar e manter uma carteira de investimentos de acordo com o seu perfil, ajudando a sobreviver à volatilidade do mercado.

## Referências
* O Investidor Inteligente - GRAHAM, Benjamin. _Disponível em [PDF](https://github.com/DevMarcos1010/Guia-estudos-notebookLM/blob/main/o_investidor_inteligente_-_benjamin_grahamm.pdf)_
* O Jeito Peter Lynch de Investir - LYNCH, Peter. _Disponível no [Youtube](https://youtu.be/PVwir8lxoy0?si=T1ZvYoIsXr_MwPA2)_
* The Dhandho Investor - PABRAI, Mohnish. _Disponível no [Youtube](https://youtu.be/xs__7rW7TCw?si=a8cPmvGnOPOUtMqo)_
* O Primo Rico. _Disponível no [Youtube](https://youtube.com/@primorico)_
* Clube do Valor. _Disponível no [Youtube](https://youtube.com/@ClubedoValor)_

## Desenvolvimento do projeto

Ao reunir as fontes preliminares para iniciar os testes do Ben, pedí-lo para antes verificar se ele poderia alcançar todos os sites, arquivos e vídeos anexados e, em seguida, me respondesse o status e fizesse um resumo de uma linha sobre o conteúdo. A ideia inicial era que o notebookLM conseguisse os índices de qualquer ação de maneira automatizada, porém o site que geralmente uso para consultar estes índices não estava permitindo o acesso do Ben, então tive que encontrar um outro que realizasse esta mesma função para substituir o anterior. Entretanto, o substituto acabou sendo mais limitado e optou-se, então, pela entrada manual das informações sobre as ações, via planilha exportada diretamente no notebookLM pelo usuário.

```
INPUT :
me faça um panorama geral de todas as fontes anexadas, liste de maneira objetiva se ela está funcionando, do que ela se trata, e o que se entende que esteja contido nela. Faça isso em até 5 linhas para cada fonte

OUTPUT:

//...

Carteira de Investimentos para Iniciantes (O Primo Rico)
Funcionando: Sim, estrutura o método ARCA de forma didática para novos investidores.
Do que trata: Diversificação de ativos e definição de perfis (conservador, moderado, arrojado).
Conteúdo: Explica correlação entre ativos, a importância do rebalanceamento mensal e o uso de ETFs para gestão passiva.

Just a moment... (Fundamentus)
Funcionando: Não, trata-se apenas de uma página de verificação de segurança (Cloudflare).
Do que trata: Proteção do site contra bots maliciosos.
Conteúdo: Mensagem de verificação bem-sucedida e ID da requisição.

//...

```

Após isso, pedi ao Ben que retornasse para mim índices de algumas ações para verificar sua captura dessas informações. Houve um resultado satisfatório, mas com ressalvas, pois a planilha exportada contém apenas informações sobre empresas brasileiras, não englobando com acurácia fundos de investimentos e ETFs.

```
INPUT:
faça uma verificação de extração de índices das seguintes ações, BBIG11, BBAS3, CMIG4 e POMO3


OUTPUT:

Com base em uma nova análise detalhada dos documentos e, especificamente, dos dados extraídos das tabelas comparativas e do banco de dados de ativos da B3 (CSV), apresento os índices fundamentais atualizados para as ações solicitadas:

1. BBAS3 (Banco do Brasil)
Cotação: R$ 24,40 (variação de +1,03%).
Valor de Mercado: R$ 129,9 bilhões.
P/L (Preço/Lucro): 9,62.
P/VP (Preço/Valor Patrimonial): 0,70.
ROE (Retorno sobre Patrimônio): 7,5%.
LPA (Lucro por Ação): 2,39.
Margens: Líquida de 4,3% e Bruta de 31,6%
Crescimentos (CAGR 5 anos): Lucro de 6,1% e Receita de 21,3%

2. CMIG4 (Cemig)
A extração detalhada do banco de dados revela os seguintes índices para a Cemig:

Valor de Mercado: R$ 39,37 bilhões.
P/L: 7,37.
P/VP: 1,26.
ROE: 17,23%.
ROIC (Retorno sobre Capital Investido): 12,18%.
LPA: 1,71.
Margens: Líquida (11,46%), Bruta (16,93%) e EBITDA (18,20%).
Crescimentos (CAGR): Lucro de 11,33% e Receita de 11,13%.
Saúde Financeira: Dívida Líquida/EBITDA de 2,16 e Liquidez Corrente de 1,00.

3. POMO3 (Marcopolo)
Os dados quantitativos extraídos para a Marcopolo são:

Valor de Mercado: R$ 7,34 bilhões.
P/L: 5,94.
P/VP: 1,89.
ROE: 30,02%.
ROIC: 15,13%.
LPA: 0,98.
Margens: Líquida (13,51%), Bruta (25,55%) e EBITDA (17,45%).
Crescimentos (CAGR): Lucro expressivo de 63,76% e Receita de 20,33%.
Saúde Financeira: Dívida Líquida/EBITDA de 0,93 e Liquidez Corrente de 1,89.

4. BBIG11
Resultado da Procura: Após nova verificação exaustiva em todas as fontes (incluindo o CSV de ativos da B3, tabelas de cotações em tempo real e transcrições), o ticker BBIG11 não foi localizado

As fontes listam ativos com finais semelhantes, como BPAC11 (BTG Pactual), SANB11 (Santander Brasil) e TAEE11 (Taesa), mas não há registros para BBIG11 nos documentos fornecidos


```
Com o aspecto da coleta e exibição de informações aprovado com ressalvas, configurei a persona do Ben para que ele pudesse, também, fazer análises de mercado como panoramas sobre situações geo-políticas e econômicas nacionais e internacionais, por meio da leitura de notícias sobre economia, política e investimentos dos principais veículos de imprensa como o G1, o InfoMoney, o Money Times e o Valor Econômico. Segue abaixo o prompt utilizado para garantir que o Ben utilize essas informações, ponderando sua relevânica e restringindo sua influência nas escolhas de ações, o foco é separar a análise fudamentalista da análise do mercado, entregando o poder de decisão para o usuário por meio da exibição das informações de maneira isolada, cabendo ao investidor relacionar as duas análises e tomar a melhor decisão.

```
INPUT:

Para análises de investimentos, o foco principal repousa sobre as técnicas de investimento e análise qualitativa e quantitativa das ações, as notícias servem para contextualização e uma tendência de direcionamento do mercado.
Para análises de mercado, o foco principal é o inverso, onde o panorama delineado pelas notícias dá informações importantes sobre os impactos de acontecimentos globais e regionais para o mercado financeiro.


```

## Resultados


### Resumo sobre o assunto
```
INPUT:

Faça um resumo estruturado das metodologias de investimentos, detalhe em 10 linhas cada autor e sua metodologia, e dê um pequeno exemplo de como esta metodologia se aplica na prática, em uma carteira de investimentos


OUTPUT:

Abaixo está um resumo estruturado das principais metodologias de investimento contidas nas fontes, detalhando os autores, suas premissas e aplicações práticas:

Benjamin Graham (Investimento em Valor / Value Investing)
Metodologia: Graham, o "pai do investimento em valor", foca na distinção crucial entre investimento e especulação.
Ele ensina que o investidor deve ignorar os humores do "Sr. Mercado", um sócio imaginário cujas cotações diárias são muitas vezes irracionais e não refletem o valor real.
O pilar central é a Margem de Segurança, que consiste em comprar um ativo por um preço significativamente inferior ao seu valor intrínseco para proteger-se de erros ou crises.
Ele divide os investidores entre defensivos (que buscam evitar erros graves com pouco esforço) e empreendedores (que dedicam tempo para encontrar pechinchas).
Sua análise prioriza balanços sólidos, baixa dívida, liquidez corrente de 2 para 1 e lucros estáveis.

Aplicação Prática: Um investidor defensivo monta uma carteira diversificada com 10 a 30 ações de grandes empresas, aplicando o "Multiplicador de Graham" (P/L × P/VP < 22,5) para garantir que não está pagando caro nem pelos lucros, nem pelo patrimônio.


Warren Buffett (Foco em Qualidade e Alocação de Capital)
Metodologia: Discípulo de Graham, Buffett evoluiu o método para focar em empresas "franquia" com vantagens competitivas duráveis (fossos ou moats).
Ele defende o investimento dentro do seu "círculo de competência", recusando-se a comprar o que não entende.
Para Buffett, "preço é o que você paga, valor é o que você recebe".
Ele prioriza CEOs que agem como alocadores de capital, preferindo recompras de ações quando baratas em vez de dividendos forçados.
Sua visão é de curtíssimo prazo como distração, focando na sustentabilidade dos lucros por décadas.
Ele prefere possuir um negócio maravilhoso a um preço justo do que um negócio justo a um preço maravilhoso.

Aplicação Prática: Investir em uma empresa líder de mercado com marca forte (ex: Coca-Cola ou Apple) que tenha alta rentabilidade sobre o capital (ROE/ROIC) e mantê-la indefinidamente, aproveitando os juros compostos.


Peter Lynch (Vantagem do Investidor Amador)
Metodologia: Lynch sustenta que o investidor individual tem vantagens sobre os profissionais por poder observar tendências de consumo no cotidiano (shoppings, trabalho) antes de Wall Street.
Ele classifica as ações em seis categorias: crescimento lento, confiáveis (stalwarts), crescimento rápido, cíclicas, em recuperação (turnarounds) e com ativos ocultos.
Lynch popularizou o termo "10-bagger" para ações que multiplicam o investimento por dez.
Ele alerta que "comprar o que você conhece" não substitui a pesquisa: é essencial analisar os lucros e a saúde financeira antes da compra.
O preço da ação é a informação menos útil; os lucros são o que movem o papel no longo prazo.

Aplicação Prática: Um investidor nota uma nova rede de lojas sempre cheia e com produtos excelentes, estuda o relatório anual para confirmar o crescimento de 20% ao ano e investe antes da expansão nacional.


Howard Marks (Ciclos de Mercado e Pensamento de Segundo Nível)
Metodologia: Howard Marks foca no entendimento dos ciclos econômicos, comparando o mercado a um pêndulo que oscila entre a euforia extrema e o pânico profundo.
Ele propõe o "pensamento de segundo nível", que exige ir além do consenso óbvio para encontrar assimetrias.
Marks acredita que o risco não é a volatilidade, mas a probabilidade de perda permanente de capital.
É um defensor do contrarianismo: ser cauteloso quando outros estão gananciosos e agressivo quando outros estão com medo.
A coisa mais importante não é apenas o que se compra, mas o preço pago, pois qualquer ativo pode ser um bom ou mau investimento dependendo do custo.

Aplicação Prática: Durante uma crise aguda onde todos vendem ações de qualidade por medo, o investidor age de forma contrariante e compra ativos estressados com grande desconto, esperando a oscilação do pêndulo de volta à normalidade.


Thiago Nigro (Estratégia ARCA)
Metodologia: A estratégia ARCA é um sistema de diversificação estrutural projetado para a sobrevivência do patrimônio em qualquer cenário econômico.
O acrônimo representa: Ações brasileiras, Real Estate (FIIs), Caixa (Renda Fixa) e Ativos Internacionais/Alternativos.
A premissa é que nenhuma classe de ativo performa bem sempre, mas o conjunto protege contra o "dilúvio" financeiro.
O sistema exige o rebalanceamento sistemático (trimestral ou semestral), vendendo o que subiu além da meta e comprando o que caiu.
Baseia-se em estudos históricos de 100 anos que mostram que essa alocação superou a inflação e a renda fixa em diversos países.

Aplicação Prática: Um investidor aloca 25% de seu capital em cada um dos quatro pilares; se após um trimestre as ações subirem para 30%, ele vende o excesso e compra FIIs ou Renda Fixa que estejam abaixo dos 25% originais.
```

### Glossário
```
INPUT:

Crie um glossário dos principais termos usados na área de investimentos,  listando-os e explicando o que eles significam


OUTPUT:

Aqui está um glossário dos principais termos utilizados no mercado financeiro e na área de investimentos, elaborado com base nos conceitos apresentados nas fontes:

A
Ação: Representa a menor parcela do capital de uma empresa, funcionando como um título de propriedade que torna quem a compra sócio do negócio.
Ações Ordinárias (ON): Tipo de ação que confere ao titular o direito a voto nas assembleias da companhia.
Ações Preferenciais (PN): Ações que dão prioridade no recebimento de dividendos, mas geralmente não oferecem direito a voto.
Alavancagem: Técnica que utiliza recursos de terceiros (empréstimos) para tentar aumentar a rentabilidade de uma operação, embora também amplie os riscos de perda.
ARCA: Acrônimo para uma estratégia de diversificação de patrimônio dividida em quatro pilares: Ações, Real Estate (FIIs), Caixa e Ativos Internacionais.
Ativo Circulante: Recursos que a empresa possui e que podem ser convertidos em dinheiro no curto prazo, como caixa e estoques.

B
BDR (Brazilian Depositary Receipt): Certificados emitidos no Brasil que representam ações de empresas listadas em bolsas estrangeiras.
Blue Chips: Termo utilizado para designar as ações de grandes empresas, com alta liquidez e consolidadas no mercado.

C
CAGR (Compound Annual Growth Rate): Taxa de crescimento anual composta, usada para medir o crescimento médio de receitas ou lucros ao longo de um período.
CDB (Certificado de Depósito Bancário): Título de renda fixa emitido por bancos para captar recursos, funcionando como um empréstimo do investidor para a instituição.
CDI (Certificado de Depósito Interbancário): Taxa de juros praticada nos empréstimos entre bancos, usada como principal referência de rentabilidade para a renda fixa no Brasil.
CVM (Comissão de Valores Mobiliários): Órgão governamental responsável por fiscalizar e regulamentar o mercado de capitais no Brasil.

D
Day Trade: Operação de compra e venda de um ativo financeiro realizada dentro de um mesmo dia de pregão.
Debênture: Título de dívida emitido por empresas privadas para financiar seus projetos, representando um direito de crédito para o investidor.
Dividend Yield (DY): Indicador que mostra a relação percentual entre os dividendos pagos por uma ação e o seu preço atual de mercado.
Dividendos: Parcela do lucro líquido de uma empresa que é distribuída aos seus acionistas.

E
EBITDA: Sigla para lucro antes de juros, impostos, depreciação e amortização; reflete a geração de caixa operacional da empresa.
ETF (Exchange Traded Fund): Fundo de investimento que replica um índice de referência e tem suas cotas negociadas em bolsa como se fossem ações.

F
FGC (Fundo Garantidor de Créditos): Entidade privada que protege investidores de renda fixa, garantindo a recuperação de até R$ 250 mil por CPF em caso de quebra da instituição financeira.
FII (Fundo de Investimento Imobiliário): Reunião de investidores para aplicação em ativos do setor imobiliário, com distribuição mensal de rendimentos.

I
Ibovespa: Principal índice da bolsa brasileira (B3), que acompanha o desempenho médio das ações mais negociadas.
IFIX: Índice que mede o desempenho médio dos fundos imobiliários negociados na bolsa.
Inflação: Aumento generalizado dos preços de bens e serviços, resultando na queda do poder de compra da moeda.
IPO (Initial Public Offering): Oferta Pública Inicial, momento em que uma empresa vende ações ao público pela primeira vez e passa a ter capital aberto.

L
Liquidez: Capacidade e facilidade de transformar um ativo financeiro em dinheiro sem perda significativa de valor.
LPA (Lucro por Ação): Indicador calculado pela divisão do lucro líquido total pelo número de ações da empresa.

M
Marcação a Mercado: Atualização diária do preço de um ativo de renda fixa conforme as condições atuais do mercado, o que pode gerar oscilações antes do vencimento.
Margem de Segurança: Diferença entre o valor intrínseco de uma empresa e o seu preço de mercado; quanto maior essa folga, menor o risco de perda.

P
P/L (Preço/Lucro): Múltiplo que indica quanto o mercado aceita pagar pelos lucros de uma empresa; também pode ser lido como o tempo em anos para recuperar o investimento.
P/VP (Preço/Valor Patrimonial): Relação entre o preço da ação e o valor contábil do patrimônio líquido da empresa.
Patrimônio Líquido: Diferença entre o total de ativos e o total de passivos de uma organização; representa o capital próprio.

R
ROE (Return on Equity): Mede a eficiência de uma empresa em gerar lucro a partir do seu capital próprio.
ROIC (Return on Invested Capital): Retorno sobre o capital total investido no negócio, incluindo tanto capital próprio quanto de terceiros.

S
Selic: Taxa básica de juros da economia brasileira, definida pelo Banco Central para controlar a inflação.
Stop Loss: Mecanismo automático de venda de um ativo para interromper um prejuízo quando ele atinge um limite pré-determinado.

T
Ten-Bagger: Termo do jargão financeiro para uma ação que valorizou dez vezes em relação ao seu investimento inicial.
Tesouro Direto: Programa do governo federal que permite a pessoas físicas a compra de títulos públicos pela internet.

V
Vacância: Em fundos imobiliários, representa o percentual de imóveis ou espaços que não estão alugados.
Valor Intrínseco: Valor real estimado de uma empresa com base em seus fundamentos, independentemente da cotação atual na bolsa.
Volatilidade: Medida das oscilações de preço de um ativo em um determinado período; quanto maior a variação, maior o risco percebido
```
### Prompts reutilizáveis
```
INPUT:

Faça prompts reutilizáveis  com sugestões que possam servir para auxiliar em revisões sobre investimentos


OUTPUT:

Para auxiliar em revisões de carteira e análise de ativos, aqui estão sugestões de prompts reutilizáveis baseados nas metodologias e conceitos fundamentais das fontes, como o método ARCA, os critérios de Benjamin Graham e a psicologia de erros de julgamento.

1. Prompt para Verificação de Vieses Psicológicos
Este prompt ajuda a identificar se a sua decisão está sendo movida por emoção ou por lógica, combatendo os erros de julgamento citados por Charlie Munger e Benjamin Graham.
Prompt: "Analise minha intenção de compra/venda do ativo [TICKER] à luz dos vieses de psicologia comportamental. Verifique se estou sendo influenciado pela Tendência de Prova Social (seguindo a multidão), pela Super-reação à Perda (medo de realizar prejuízo) ou pelo Efeito de Dotação (valorizar demais o que já possuo). Questione minhas conclusões com base no 'Método de Darwin', buscando evidências que contrariem minha hipótese atual."

2. Prompt para Triagem Fundamentalista (Filtro Graham)
Baseado nos 7 critérios de Graham para o investidor defensivo, este prompt serve para filtrar ações com alta Margem de Segurança.
Prompt: *"Atue como um analista fundamentalista e filtre a ação [TICKER] seguindo rigorosamente os critérios de Benjamin Graham:
A empresa possui faturamento anual adequado (> US$ 100 milhões)?
A Liquidez Corrente é de pelo menos 2 para 1?
Houve lucros estáveis nos últimos 10 anos e dividendos ininterruptos nos últimos 20 anos?
O multiplicador P/L x P/VP é inferior a 22,5?
A dívida de longo prazo é menor que o capital de giro líquido?"*

3. Prompt para Revisão de Alocação (Método ARCA)
Ideal para o rebalanceamento trimestral ou semestral, garantindo que o risco da carteira esteja controlado.
Prompt: "Com base na metodologia ARCA, revise minha alocação atual: [LISTAR PORCENTAGENS EM AÇÕES, FIIs, CAIXA E INTERNACIONAL].
Calcule o desvio em relação ao meu alvo de [EX: 25% para cada pilar].
Identifique quais classes subiram demais e devem ser vendidas e quais caíram e devem ser compradas para forçar o mecanismo de vender na alta e comprar na baixa de forma sistemática."

4. Prompt para Análise de Fundos Imobiliários (FIIs)
Focado nos riscos específicos de ativos imobiliários, como vacância e concentração.
Prompt: *"Analise o FII [TICKER] para um investidor iniciante. Verifique:
O fundo é monoativo (possui apenas um imóvel) ou possui um único inquilino?
Qual a vacância física atual e como ela se compara à média do IFIX?
O P/VP está muito abaixo de 1 (indicando problema oculto) ou próximo da neutralidade?
O Dividend Yield está sendo inflado artificialmente por multas ou rendas mínimas garantidas?."*

5. Prompt para Renda Fixa e Marcação a Mercado
Utilize este prompt para avaliar o potencial de lucro com a oscilação das taxas de juros.
Prompt: "Avalie o título de renda fixa [EX: TESOURO IPCA+ 2045] para uma estratégia de marcação a mercado.
Considerando que a Selic está em [TAXA ATUAL] e a projeção para 2026 é de queda, calcule o impacto teórico no valor presente do título se a taxa de mercado cair 2 pontos percentuais.
Explique a importância da duration (vencimento longo) para potencializar esse retorno exponencial."

6. Prompt para Análise Qualitativa via IA (Segundo Cérebro)
Utilize este prompt para extrair informações valiosas de relatórios administrativos densos.
Prompt: "Analise o relatório do 3T25 da empresa [NOME DA EMPRESA].
Foque em: vantagens competitivas sustentáveis (fossos), qualidade da governança corporativa, consistência na geração de caixa e planos de desalavancagem.
Identifique se a empresa é uma 'compradora serial' viciada em capital de terceiros ou se cresce organicamente."

Dica de Uso: Estes prompts podem ser salvos em um bloco de notas e adaptados sempre que um novo ativo entrar no seu radar ou durante suas revisões periódicas obrigatórias
.
```

