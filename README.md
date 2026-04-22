# Ben, o notebookLM de investimentos

Ao explorar as capacidades do notebookLM e refletir sobre suas aplicações no cotidiano, surgiu a necessidade - e oportunidade - de iniciar um projeto que envolvesse uma dor minha. Um dos meus hobbies é nada mais do que operar uma pequena carteira de investimentos na B3, e uma dificuldade real do meu passatempo é fazer uma análise fundamental de ações, uma vez que no mercado mobiliário brasileiro existem centenas, até milhares de empresas, e encontrar a "melhor" é como tentar achar uma agulha no palheiro.

Para me ajudar com isso, criei um notebookLM que me ajudasse que essa tarefa, o Ben (para facilitar as referências), um modelo de linguagem especialista em análise fundamentalista de ações. O objetivo deste notebookLM é auxiliar o investidor na filtragem de ações, seguindo metodologias bastante usadas no mercado, como as de Benjamin Graham, em "O investidor inteligente", e de outros autores renomados na área de investimentos como Peter Lynch e Mohnish Pabrai, além de influenciadores famosos como o Thiago Nigro, d'O Primo Rico, e Ramiro Gomes, do Clube do Valor. E além disso, com os ensinamentos destas personalidades e com acesso às notícias globais de economia, a gerenciar e manter uma carteira de investimentos de acordo com o seu perfil, ajudando a sobreviver à volatilidade do mercado.

## Referências
* O Investidor Inteligente - GRAHAM, Benjamin. _Disponível em [PDF](https://github.com/DevMarcos1010/Guia-estudos-notebookLM/blob/main/o_investidor_inteligente_-_benjamin_grahamm.pdf)_
* O Jeito Peter Lynch de Investir - LYNCH, Peter. _Disponível no [Youtube](https://youtu.be/PVwir8lxoy0?si=T1ZvYoIsXr_MwPA2)_
* The Dhandho Investor - PABRAI, Mohnish. _Disponível no [Youtube](https://youtu.be/xs__7rW7TCw?si=a8cPmvGnOPOUtMqo)_
* O Primo Rico. _Disponível no [Youtube](https://youtube.com/@primorico)
* Clube do Valor. _Disponível no [Youtube](https://youtube.com/@ClubedoValor)

## Desenvolvimento do projeto

Ao reunir as fontes preliminares para iniciar os testes do Ben, pedí-lo para antes verificar se ele poderia alcançar todos os sites, arquivos e vídeos anexados e, em seguida, me respondesse o status e fizesse um resumo de uma linha sobre o conteúdo. A ideia inicial era que o notebookLM conseguisse os índices de qualquer ação de maneira automatizada, porém o site que geralmente uso para consultar estes índices não estava permitindo o acesso do Ben, então tive que encontrar outro site que realizasse esta mesma função para substituir o anterior. Entretanto, o substituto acabou sendo mais limitado e optou-se, então, pela entrada manual das informações sobre as ações, via planilha exportada diretamente no notebookLM pelo usuário.

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





