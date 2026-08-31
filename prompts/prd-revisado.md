# PRD — Aplicativo Conversacional de Organização de Finanças Pessoais

**Status:** Documento de Requisitos do Produto  
**Versão:** 1.0  
**Idioma da experiência:** Português brasileiro  
**Plataforma inicial:** Aplicação web responsiva  
**Contexto de uso:** Exercício de Vibe Coding no Lovable  

## 1. Visão do produto

Criar um aplicativo de organização de finanças pessoais que permita ao usuário registrar, consultar e compreender sua vida financeira por meio de conversas em linguagem natural. A experiência deve ser simples, acolhedora, educativa e acessível, reduzindo a necessidade de formulários manuais, planilhas e conhecimentos prévios sobre finanças.

O produto funcionará como um **assistente financeiro pessoal de caráter educativo**. Ele poderá organizar informações, identificar padrões, acompanhar metas e sugerir possibilidades de economia, mas não deverá se apresentar como consultor financeiro, contador ou profissional que toma decisões pelo usuário.

A conversa será a interface principal. O usuário poderá escrever mensagens como “gastei R$ 42,90 no mercado hoje”, “quanto ainda posso gastar este mês?” ou “quero guardar R$ 1.200 até dezembro”. O aplicativo deverá interpretar a intenção, pedir esclarecimentos quando necessário e transformar a conversa em dados financeiros estruturados.

## 2. Problema

Muitas pessoas abandonam o controle financeiro porque as soluções existentes exigem registros frequentes, preenchimento de vários campos, categorização manual e interpretação de gráficos complexos. Para iniciantes, essa fricção torna a atividade cansativa, confusa ou difícil de manter.

O produto deve reduzir essa barreira por meio de uma interação natural, confirmações claras, visualizações simples e orientações que não julguem o comportamento do usuário. A pessoa deve conseguir começar rapidamente, entender o que foi registrado e corrigir informações sem perder o controle sobre seus próprios dados.

## 3. Objetivo do produto

Permitir que uma pessoa registre e compreenda suas movimentações financeiras com o mínimo de esforço, utilizando uma conversa acessível como principal interface, sem retirar a possibilidade de revisar, editar, exportar ou excluir seus dados.

### 3.1 Objetivos específicos

| Objetivo | Resultado esperado |
|---|---|
| Reduzir a fricção de registro | O usuário consegue cadastrar uma receita ou despesa em uma única mensagem, sem formulário extenso. |
| Aumentar a clareza financeira | O aplicativo apresenta receitas, despesas, saldo, categorias e metas em linguagem simples. |
| Apoiar a criação de hábitos | O sistema oferece lembretes e recomendações configuráveis, sem excesso de notificações ou tom de cobrança. |
| Preservar a autonomia | O usuário confirma, corrige, edita, exporta e exclui seus dados sempre que necessário. |
| Promover inclusão | A experiência atende ao maior número possível de pessoas, considerando diferentes capacidades, dispositivos, contextos e níveis de familiaridade digital. |

## 4. Princípios do produto

### 4.1 Conversa antes de formulário

A conversa deve ser o caminho principal para registrar transações e fazer consultas. Formulários, filtros e telas de edição devem continuar disponíveis como alternativas, mas não podem ser obrigatórios para as tarefas mais frequentes.

### 4.2 Simplicidade sem perda de controle

A interface deve esconder complexidade desnecessária, mas nunca ocultar informações importantes. Sempre que o sistema interpretar uma mensagem, o usuário deverá conseguir visualizar o que foi entendido e confirmar ou corrigir os dados.

### 4.3 Educação sem julgamento

O aplicativo deve usar linguagem respeitosa, neutra e encorajadora. Não deve presumir irresponsabilidade, criticar hábitos de consumo, utilizar culpa como mecanismo de engajamento ou associar saúde financeira ao valor pessoal do usuário.

### 4.4 Privacidade por padrão

Dados financeiros são sensíveis. O produto deve coletar somente o necessário, explicar por que cada informação é solicitada e oferecer controles claros para edição, exclusão e exportação dos dados.

### 4.5 Design Universal

O produto deve adotar **Design Universal** como requisito estrutural. Isso significa criar uma experiência que possa ser utilizada, compreendida e acessada pelo maior número possível de pessoas, em diferentes dispositivos, contextos, idades, níveis de familiaridade tecnológica e capacidades sensoriais, motoras e cognitivas.

O Design Universal não deve ser tratado como correção posterior. Desde o início, a interface deverá oferecer caminhos equivalentes para concluir tarefas, combinar texto e recursos visuais sem depender exclusivamente de uma única modalidade e permitir a personalização de aspectos relevantes da experiência.

A implementação deve buscar conformidade com as [Web Content Accessibility Guidelines — WCAG 2.2, nível AA][1], quando aplicável, sem limitar o objetivo mais amplo de proporcionar uma experiência inclusiva, flexível e fácil de usar.

### 4.6 Transparência da inteligência artificial

O usuário deve saber quando está interagindo com uma interpretação ou recomendação gerada por inteligência artificial. O aplicativo deve diferenciar dados confirmados pelo usuário de sugestões, estimativas e inferências do sistema.

## 5. Público-alvo

O público principal é formado por pessoas que desejam começar a organizar suas finanças ou que já tentaram usar planilhas e aplicativos tradicionais, mas abandonaram a prática por considerá-la trabalhosa ou confusa.

O produto deve atender especialmente a quem prefere escrever ou falar em linguagem natural, tem pouco conhecimento de conceitos financeiros, acessa o serviço principalmente pelo celular ou precisa de uma interface com baixa carga cognitiva.

### 5.1 Perfis prioritários

| Perfil | Necessidade | Implicação para o produto |
|---|---|---|
| Iniciante | Entender para onde o dinheiro está indo sem aprender uma ferramenta complexa. | Termos simples, exemplos, explicações curtas e orientação passo a passo. |
| Pessoa com rotina corrida | Registrar gastos rapidamente durante o dia. | Poucos passos, confirmação objetiva e edição posterior. |
| Pessoa que abandonou planilhas | Retomar o controle sem sentir que está recomeçando uma tarefa pesada. | Cadastro gradual, visão resumida e ausência de cobrança moral. |
| Pessoa com necessidade de acessibilidade | Interagir com diferentes recursos de entrada e saída. | Contraste adequado, teclado, leitor de tela, texto redimensionável, alvos de toque amplos e alternativas à cor, ao áudio e ao gesto. |

## 6. Proposta de valor

> “Organize sua vida financeira conversando, entenda seus hábitos com clareza e avance nas suas metas no seu próprio ritmo.”

O diferencial do produto é combinar conversa, confirmação, visualização e educação em uma experiência coerente. A inteligência artificial não deve apenas interpretar mensagens, mas também tornar o controle financeiro mais compreensível, reversível e inclusivo.

## 7. Escopo funcional

### 7.1 Cadastro e configuração inicial

O usuário deve poder iniciar a experiência com uma configuração curta e progressiva. O primeiro acesso não deve exigir o preenchimento de todas as informações financeiras. Deve ser possível começar registrando uma única transação e completar o perfil posteriormente.

A configuração pode solicitar nome ou forma de tratamento, moeda padrão, ciclo mensal, categorias preferidas, renda recorrente opcional e metas iniciais. Cada campo deve indicar se é obrigatório ou opcional.

### 7.2 Registro de transações por conversa

O usuário deve conseguir registrar receitas e despesas em linguagem natural, utilizando texto e, quando disponível e autorizado, voz. O sistema deve interpretar, no mínimo, tipo da movimentação, valor, data, descrição, categoria e observação.

Exemplos de mensagens válidas:

- “Gastei R$ 35,90 no almoço hoje.”
- “Recebi R$ 2.500 de salário ontem.”
- “Paguei 89 reais de internet este mês.”
- “Comprei um presente de R$ 120 no cartão.”

Quando os dados essenciais estiverem claros, o sistema deve exibir uma prévia para confirmação. Quando faltar uma informação importante, deve fazer uma pergunta objetiva, sem repetir dados já fornecidos.

Se houver ambiguidade, o aplicativo deve apresentar alternativas compreensíveis. A baixa confiança em uma categoria ou data não deve impedir o registro, mas deve ser explicitada e resolvida pelo usuário ou deixada para edição posterior.

### 7.3 Categorização automática

O sistema deve sugerir uma categoria com base na descrição e, quando apropriado, no histórico do usuário. A categoria sugerida deve ser apresentada como sugestão, não como fato imutável.

As categorias iniciais devem ser simples e editáveis: alimentação, moradia, transporte, saúde, educação, lazer, compras, assinaturas, contas, renda, transferências e outros.

O usuário deve poder criar, renomear, mesclar ou desativar categorias sem perder indevidamente o histórico das transações. A ausência de categoria nunca deve impedir o registro.

### 7.4 Consulta, edição e exclusão

O usuário deve conseguir fazer perguntas em linguagem natural, por exemplo: “quanto gastei com transporte este mês?” ou “mostre minhas despesas de sábado”. As respostas devem informar o período considerado e, quando possível, oferecer acesso à lista de transações que originou o resultado.

Também deve ser possível consultar as transações em uma lista pesquisável e filtrável, editar qualquer campo, duplicar uma movimentação recorrente e excluir um registro. A exclusão exige confirmação clara e, quando apropriado, deve oferecer uma alternativa de arquivamento.

### 7.5 Metas financeiras

O usuário deve poder criar metas com nome, valor-alvo, valor já reservado, prazo e observação opcional. Exemplos incluem montar uma reserva, fazer uma viagem, quitar uma dívida ou comprar um item.

O sistema deve exibir o progresso da meta de maneira compreensível. Quando houver dados suficientes, poderá sugerir um valor periódico necessário para alcançar o objetivo, deixando claro que se trata de uma estimativa.

O usuário deve poder pausar, editar, concluir ou excluir uma meta. O aplicativo não deve tratar o não cumprimento como fracasso pessoal nem alterar o saldo automaticamente por causa da existência de uma meta.

### 7.6 Agente Financeiro

O “Agente Financeiro” é o componente conversacional que interpreta mensagens, responde perguntas, orienta o uso do produto e apresenta recomendações educativas de economia.

As recomendações devem ser baseadas nos dados disponíveis, explicar brevemente o motivo da sugestão e permitir que o usuário peça mais detalhes. O agente deve preferir expressões como “uma possibilidade é” e “se fizer sentido para você”, evitando ordens categóricas.

O agente não deve inventar transações, saldos, fontes de renda ou dados ausentes. Quando não houver informação suficiente, deverá declarar a limitação e pedir os dados necessários. Também deve evitar aconselhamento personalizado de investimento, crédito, impostos, seguros ou decisões financeiras de alto risco.

### 7.7 Relatórios e visualizações

O aplicativo deve oferecer uma visão geral simples do período selecionado, com saldo, receitas, despesas, evolução das metas e principais categorias de gasto. O usuário deve poder alternar entre semana, mês e intervalo personalizado.

Os relatórios devem priorizar compreensão e ação. Cada gráfico ou indicador deve ter título descritivo, resumo textual e valores acessíveis sem depender exclusivamente da interpretação visual. A cor não pode ser o único meio de diferenciar categorias ou estados.

O usuário deve poder acessar os detalhes de cada total apresentado e exportar seus próprios dados em formato estruturado, como CSV, quando essa função estiver disponível.

### 7.8 Lembretes e notificações

O usuário deve poder ativar, desativar e configurar lembretes para registrar movimentações, acompanhar metas ou revisar o período financeiro. As notificações devem ser discretas, úteis e respeitar a frequência escolhida.

O produto não deve enviar mensagens alarmistas, coercitivas ou culpabilizadoras. O usuário deve poder silenciar temporariamente todas as notificações.

## 8. Requisitos funcionais priorizados

| ID | Requisito | Prioridade | Critério de aceitação |
|---|---|---|---|
| RF-01 | Registrar receita ou despesa por mensagem em linguagem natural. | Essencial | Uma mensagem válida gera uma prévia estruturada para confirmação. |
| RF-02 | Solicitar somente dados ausentes ou ambíguos. | Essencial | O sistema não repete perguntas já respondidas na mesma interação. |
| RF-03 | Confirmar, corrigir ou cancelar um registro interpretado. | Essencial | Nenhuma transação ambígua é salva sem ação clara do usuário. |
| RF-04 | Sugerir categoria automaticamente. | Essencial | A sugestão pode ser aceita ou alterada antes ou depois do salvamento. |
| RF-05 | Listar, buscar, filtrar, editar e excluir transações. | Essencial | O usuário consegue localizar uma transação e modificar seus dados. |
| RF-06 | Consultar totais e transações por conversa. | Essencial | A resposta informa o período e permite verificar os registros considerados. |
| RF-07 | Criar e acompanhar metas financeiras. | Essencial | A meta exibe valor-alvo, progresso, prazo e estado atual. |
| RF-08 | Exibir resumo financeiro e relatórios simples. | Essencial | O resumo pode ser compreendido sem conhecimento técnico de finanças. |
| RF-09 | Fornecer dicas educativas contextualizadas. | Importante | A dica apresenta contexto, linguagem não julgadora e opção de ignorar. |
| RF-10 | Gerenciar categorias. | Importante | O usuário personaliza a taxonomia sem apagar o histórico indevidamente. |
| RF-11 | Configurar lembretes. | Importante | O usuário controla ativação, frequência e silenciamento. |
| RF-12 | Oferecer entrada e saída compatíveis com acessibilidade. | Essencial | As principais tarefas podem ser realizadas por teclado e leitor de tela, sem depender apenas de cor, áudio ou gesto. |
| RF-13 | Exportar dados do usuário. | Importante | O usuário consegue solicitar uma cópia legível de seus próprios dados. |
| RF-14 | Exibir estados de carregamento, vazio, erro e sucesso. | Essencial | Cada estado comunica o que ocorreu e o próximo passo possível. |

## 9. Requisitos de Design Universal e acessibilidade

O Design Universal deve ser aplicado em todas as telas, fluxos, mensagens e respostas do agente. A solução deve oferecer mais de uma forma de perceber informações, interagir com controles e concluir tarefas sempre que isso for relevante.

| Área | Requisito |
|---|---|
| Percepção visual | Usar contraste suficiente, tipografia legível, espaçamento confortável e hierarquia clara. A informação não deve depender somente de cor, ícone ou posição. |
| Percepção auditiva | Todo conteúdo transmitido por áudio deve ter alternativa textual. Sons de alerta não podem ser a única indicação de erro ou sucesso. |
| Navegação por teclado | Todas as funções principais devem ser acessíveis por teclado, com foco visível, ordem lógica e saída possível de componentes interativos. |
| Leitores de tela | Utilizar semântica adequada, rótulos descritivos, mensagens de status anunciáveis e nomes acessíveis para botões, gráficos e campos. |
| Mobilidade | Usar alvos de toque amplos, evitar gestos complexos e oferecer alternativas para arrastar, deslizar ou manter pressionado. |
| Cognição e linguagem | Preferir frases curtas, vocabulário cotidiano, instruções em etapas, mensagens previsíveis e confirmação antes de ações destrutivas. |
| Personalização | Respeitar redimensionamento de texto, modo claro e escuro quando disponível, redução de movimento e preferências de notificações. |
| Dispositivos e conectividade | Garantir boa experiência em celular, tablet e desktop, com mensagens claras em conexão lenta ou interrompida. |
| Erros | Informar o que aconteceu, possível causa e como corrigir, sem culpar o usuário. Preservar dados já preenchidos sempre que possível. |
| Gráficos | Oferecer resumo textual, valores detalhados e lista ou tabela equivalente para informações que não possam depender apenas do gráfico. |

A solução deve ser avaliada com navegação por teclado, leitor de tela, zoom ou redimensionamento de texto, diferentes larguras de tela e interação exclusivamente por toque. Sempre que possível, a validação deve incluir pessoas com diferentes níveis de familiaridade digital e diferentes necessidades de acessibilidade.

## 10. Experiência conversacional

A conversa deve parecer natural, mas manter estrutura suficiente para que o usuário entenda o estado de cada ação. O agente deve distinguir entre mensagem informativa, pergunta, intenção de criar ou editar dados e solicitação de recomendação.

As respostas devem ser objetivas, apresentar uma ação principal e oferecer alternativas quando necessário. O agente deve evitar respostas longas para tarefas simples e permitir que o usuário peça explicações mais detalhadas.

### 10.1 Estados mínimos da conversa

| Estado | Comportamento esperado |
|---|---|
| Interpretando | Informar brevemente que a mensagem está sendo processada, sem bloquear a interface desnecessariamente. |
| Aguardando confirmação | Mostrar os dados interpretados e ações claras para confirmar, editar ou cancelar. |
| Registro concluído | Confirmar o que foi salvo e oferecer uma próxima ação relevante, sem excesso de sugestões. |
| Informação insuficiente | Explicar qual dado falta e fazer uma pergunta única e objetiva. |
| Baixa confiança | Mostrar interpretações possíveis e pedir uma escolha do usuário. |
| Erro técnico | Informar que a ação não foi concluída, preservar a mensagem e oferecer nova tentativa ou caminho manual. |
| Conteúdo não compreendido | Pedir reformulação com um exemplo, sem afirmar que o usuário fez algo errado. |

### 10.2 Exemplos de resposta

Para “gastei 42,90 no mercado hoje”:

> “Entendi: despesa de **R$ 42,90**, em **Alimentação**, com data de **hoje**. Quer salvar?”

Para “paguei minha conta”:

> “Qual foi o valor da conta? Se quiser, também posso registrar a data e o tipo de conta.”

Para uma recomendação:

> “Suas despesas com assinaturas aumentaram neste período. Uma possibilidade é revisar quais serviços você usa com frequência. Quer ver a lista de assinaturas registradas?”

## 11. Regras de negócio

| ID | Regra |
|---|---|
| RN-01 | Toda transação deve possuir tipo, valor e data antes de ser considerada completa. |
| RN-02 | O sistema deve aceitar transações sem categoria definida e permitir categorização posterior. |
| RN-03 | Valores devem ser armazenados com precisão adequada para moeda e exibidos no padrão brasileiro, usando vírgula para centavos. |
| RN-04 | Datas relativas, como “hoje” e “ontem”, devem ser interpretadas com base no fuso horário configurado pelo usuário. |
| RN-05 | Saldo e totais devem indicar claramente o período considerado e diferenciar receitas de despesas. |
| RN-06 | Uma interpretação gerada pelo agente não deve alterar dados sem confirmação quando houver ambiguidade ou impacto relevante. |
| RN-07 | Edição e exclusão devem ser atribuídas ao usuário autenticado e refletir nas visões relacionadas. |
| RN-08 | Metas não devem alterar o saldo automaticamente sem uma transação ou ação explícita do usuário. |
| RN-09 | Recomendações devem usar somente informações disponíveis e indicar quando forem baseadas em estimativas. |
| RN-10 | Uma falha de interpretação não pode criar silenciosamente uma transação incorreta. |

## 12. Segurança, privacidade e confiança

A aplicação deve tratar informações financeiras como dados sensíveis e adotar minimização de dados, controle de acesso e transparência sobre o uso das informações. O usuário deve conseguir consultar, editar, exportar e excluir seus dados por caminhos claros.

A interface deve informar quando uma resposta foi gerada com base em interpretação automática. O agente não deve solicitar senhas bancárias, códigos de autenticação, números completos de cartão ou outras credenciais que não sejam necessárias para o escopo definido.

Se integrações externas forem adicionadas futuramente, elas deverão ser opcionais, explicar quais permissões serão concedidas e permitir revogação. Nenhuma integração bancária deve ser presumida como parte deste documento.

## 13. Requisitos não funcionais

| Categoria | Requisito |
|---|---|
| Responsividade | A experiência deve funcionar adequadamente em celulares, tablets e desktops, priorizando conforto em telas pequenas. |
| Desempenho | A interface deve fornecer feedback imediato e não parecer travada durante processamento ou chamadas de IA. |
| Confiabilidade | Mensagens e registros não devem ser perdidos por falhas temporárias de rede ou processamento. |
| Acessibilidade | As principais tarefas devem seguir as boas práticas da WCAG 2.2 nível AA, considerando as particularidades da tecnologia utilizada. |
| Clareza | Componentes, mensagens e estados devem usar nomenclatura consistente. |
| Internacionalização | A arquitetura deve permitir futuramente outros idiomas, moedas, formatos numéricos e datas, ainda que a primeira versão use português brasileiro e real brasileiro. |
| Observabilidade | Erros técnicos devem ser investigáveis sem expor dados financeiros sensíveis em logs. |
| Manutenibilidade | Regras de interpretação, categorias, textos e componentes devem ser modulares e fáceis de alterar. |

## 14. Estrutura sugerida de telas e áreas

A arquitetura deve manter a conversa como ponto de entrada, mas oferecer caminhos alternativos para quem prefere navegar visualmente.

| Área | Finalidade |
|---|---|
| Início ou conversa | Registrar transações, fazer perguntas, receber confirmações e interagir com o Agente Financeiro. |
| Resumo financeiro | Exibir saldo, receitas, despesas, principais categorias e período selecionado. |
| Transações | Listar, buscar, filtrar, editar, excluir e revisar movimentações. |
| Metas | Criar, acompanhar, pausar, editar e concluir objetivos financeiros. |
| Relatórios | Explorar tendências e distribuições por período, com alternativas textuais aos gráficos. |
| Categorias | Personalizar categorias e revisar sugestões do sistema. |
| Notificações | Configurar lembretes, frequência e silenciamento. |
| Privacidade e configurações | Gerenciar dados, preferências de acessibilidade, idioma, moeda, fuso horário e conta. |
| Ajuda | Apresentar exemplos de mensagens, explicações de conceitos e formas de obter suporte. |

## 15. Fluxos principais

### 15.1 Primeiro registro

O usuário acessa o produto, recebe uma explicação curta e pode começar sem preencher um cadastro extenso. Ele escreve uma movimentação, revisa a interpretação, confirma o registro e visualiza o impacto no resumo financeiro.

### 15.2 Registro com informação ausente

O usuário envia uma mensagem incompleta. O agente identifica o dado essencial que falta, faz uma pergunta objetiva, incorpora a resposta e apresenta o resumo final para confirmação.

### 15.3 Correção de interpretação

O usuário percebe que a categoria ou a data está incorreta. Ele escolhe editar, modifica o campo desejado e salva. O aplicativo atualiza os totais, relatórios e recomendações afetados.

### 15.4 Criação de meta

O usuário informa o objetivo em conversa ou por formulário curto. O sistema confirma valor, prazo e progresso inicial, apresentando uma estimativa somente quando houver dados suficientes.

### 15.5 Consulta financeira

O usuário faz uma pergunta sobre período ou categoria. O aplicativo responde com o total, explicita os filtros aplicados e oferece acesso às transações que compõem o resultado.

## 16. Conteúdo e tom de voz

O tom deve ser educativo, acessível, acolhedor e direto. A comunicação deve evitar jargões ou explicá-los quando forem indispensáveis. O sistema deve falar com o usuário, e não sobre o usuário, preservando sua autonomia e dignidade.

Mensagens de erro, lembrete e recomendação devem ser úteis mesmo quando lidas isoladamente. O produto deve evitar expressões como “você está gastando errado”, “você falhou” ou “controle melhor sua vida”. Deve preferir construções como “há uma diferença em relação ao período anterior” e “podemos revisar esse registro”.

## 17. Métricas de sucesso

As métricas devem avaliar utilidade, compreensão, confiança e acessibilidade, e não somente volume de uso. Nenhuma métrica isolada deve incentivar notificações excessivas, registros incorretos ou comportamento financeiro prejudicial.

| Dimensão | Indicador sugerido |
|---|---|
| Ativação | Percentual de novos usuários que concluem o primeiro registro com sucesso. |
| Facilidade | Tempo e quantidade de interações para registrar uma transação comum. |
| Precisão percebida | Percentual de interpretações aceitas sem edição, acompanhado de revisão de qualidade. |
| Retenção de hábito | Frequência de retorno para registrar ou consultar informações, sem tratar o uso como obrigação. |
| Compreensão | Percentual de usuários capazes de explicar o resumo e os relatórios em testes de usabilidade. |
| Metas | Percentual de usuários que criam uma meta e conseguem identificar seu progresso. |
| Confiança | Avaliação sobre controle, transparência e segurança percebida. |
| Acessibilidade | Taxa de conclusão das principais tarefas usando teclado, leitor de tela, zoom, toque e diferentes tamanhos de tela. |
| Qualidade | Taxa de erros técnicos, duplicidades, interpretações incorretas e solicitações de correção. |

## 18. Critérios gerais de aceite

O produto será considerado coerente com este PRD quando uma pessoa iniciante conseguir registrar uma receita ou despesa em linguagem natural, compreender o que foi interpretado, confirmar ou corrigir o registro e localizar essa movimentação posteriormente.

Também será necessário que o usuário consiga consultar um total por período, criar uma meta, acompanhar o progresso, receber uma recomendação contextualizada e desativar lembretes sem depender de conhecimento técnico.

As principais tarefas devem permanecer compreensíveis e operáveis em telas pequenas, por teclado e com tecnologia assistiva. Gráficos e indicadores devem possuir equivalentes textuais, e nenhuma ação destrutiva deve ocorrer sem confirmação clara.

## 19. Fora de escopo

Para preservar o foco do produto, não fazem parte deste PRD, salvo decisão posterior documentada:

- integração automática com bancos, cartões ou corretoras;
- execução de pagamentos, transferências ou investimentos;
- recomendação de compra ou venda de ativos;
- aconselhamento jurídico, tributário, contábil ou de crédito;
- concessão de empréstimos ou análise de risco de crédito;
- monitoramento de contas de terceiros;
- compartilhamento público de dados financeiros;
- gamificação baseada em punição, ranking ou exposição de hábitos;
- substituição de profissionais especializados em situações financeiras complexas.

## 20. Orientações de implementação para o Lovable

A implementação deve priorizar uma experiência navegável, responsiva e acessível, com o fluxo conversacional como caminho principal. A interface deve apresentar dados demonstrativos ou persistência real conforme a capacidade do ambiente, mas não deve simular integrações financeiras reais sem deixar isso explícito.

Os componentes devem ser reutilizáveis e manter consistência entre conversa, listas, formulários, relatórios e configurações. Estados de carregamento, vazio, erro, sucesso e baixa confiança da IA devem ser tratados desde o início.

A inteligência artificial deve retornar respostas estruturadas para intenções como criar transação, consultar transações, editar registro, criar meta e solicitar recomendação. Antes de persistir dados ambíguos, a interface deve apresentar uma etapa de confirmação.

Caso o recurso de IA não esteja disponível, o produto deve mostrar uma mensagem clara e oferecer um caminho manual equivalente para as tarefas essenciais. A primeira implementação deve usar dados fictícios ou dados inseridos pelo próprio usuário, sem presumir acesso a contas bancárias.

## 21. Entregável esperado da IA no contexto do Lovable

Este documento deve ser usado como especificação do produto para orientar a construção de uma implementação navegável. A IA responsável pela implementação deve respeitar os requisitos funcionais, não funcionais, de acessibilidade, privacidade e tom de voz descritos aqui.

Antes de concluir cada fluxo, deve verificar se:

1. a conversa é compreensível para uma pessoa iniciante;
2. o usuário mantém controle sobre confirmações, edições e exclusões;
3. informações importantes não dependem somente de cor, áudio, gesto ou gráfico;
4. estados de erro, carregamento, baixa confiança e ausência de dados estão contemplados;
5. dados fictícios, limitações da IA e ausência de integrações reais estão explícitos;
6. a interface oferece boa experiência ao maior número possível de usuários, seguindo os princípios de **Design Universal**.

Este documento define requisitos e critérios de qualidade. Ele não autoriza a criação de integrações financeiras reais, recomendações de investimento ou decisões automáticas em nome do usuário.
