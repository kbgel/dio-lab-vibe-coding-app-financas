# Interações com as IAs

Este documento registra todos os prompts e interações realizados durante o desenvolvimento do conceito do app **Alvorada**.

---

## Sumário

1. [Prompt para o Copilot (revisão do PRD)](#prompt-para-o-copilot)
2. [Output do Copilot (PRD revisado — input para o Lovable)](#output-copilot)
3. [Pedidos de ajustes ao Lovable](#pedidos-de-ajustes-ao-lovable)

---

## Prompt para o Copilot

```markdown
Me ajude a revisar meu PRD (Product Requeriment Document) que pretendo usar no Lovable para exercitar minhas skills de Vibe Coding.
Deixe claro que a solução deve ter um Design Universal, ou seja, que possa ser usado com boa experiência pelo máximo de usuários possíveis.
Como resposta, me mande o apenas o PRD revisado, *não* gere o MVP.

```
# Contexto
Quero criar um aplicativo de Organização de Finanças Pessoais que funcione por meio de conversas com o usuário.  
A ideia é facilitar o controle financeiro de forma simples e natural, sem formulários manuais ou planilhas complexas.

# Problema
Muitas pessoas desistem de controlar seus gastos porque os apps atuais exigem muita entrada manual e pouca personalização.  
Quero resolver isso com uma experiência de conversa e recomendações automáticas de economia.

# Público-Alvo
Pessoas que querem começar a organizar suas finanças de forma prática e sem complicação, principalmente iniciantes.

# Funcionalidades-Chave
1. Registrar gastos via chat em linguagem natural.  
2. Classificar automaticamente as transações.  
3. Definir e acompanhar metas financeiras.  
4. Receber dicas de economia do "Agente Financeiro".  
5. Visualizar relatórios simples e personalizados.

# Entregável da IA
Gerar um plano de MVP com as principais telas, recursos necessários e um esboço de validação inicial.  
Usar tom educativo e linguagem acessível, em português.

---

## Output Copilot

O Copilot devolveu um PRD completo e estruturado com **21 seções**, incluindo:

- Visão do produto e princípios (conversa antes de formulário, Design Universal, transparência da IA)
- Público-alvo com perfis prioritários
- Escopo funcional detalhado: registro por conversa, categorização automática, metas, Agente Financeiro, relatórios, lembretes
- 14 requisitos funcionais priorizados (essencial/importante)
- Requisitos de Design Universal e acessibilidade (WCAG 2.2 AA)
- Regras de negócio, segurança e privacidade
- Experiência conversacional com estados e exemplos de resposta
- Estrutura sugerida de telas, fluxos principais e métricas de sucesso
- Orientações específicas de implementação para o Lovable

> 📄 O PRD revisado completo está disponível no arquivo original [`prd-revisado.md`](prd-revisado.md).

---

## Pedidos de ajustes ao Lovable

Após a geração inicial do MVP pelo Lovable, foram feitos ajustes pontuais para refinar a experiência:

### 1. Página Metas

```markdown
Não consigo criar nem alterar nenhuma meta através do chat com o assistente, somente manualmente.
Faça com que eu possa fazer solicitações como criação/exclusão de metas e depósitos/saques/ajuste de saldos de metas diretamente ao assistente.
Quero que ao pedir para o assistente adicionar um valor a uma meta, esse valor seja automaticamente deduzido do meu saldo. Assim como, ao sacar dinheiro de uma meta, esse valor seja adicionado ao meu saldo.
Também gostaria que a seção de ajuste manual das metas fosse organizada com as opções de depósitos/saques/ajuste de saldo ao invés de apenas a possibilidade de atualizar o valor total. Cada transação de meta também deve ficar registrada.
---
Além disso, ao clicar em concluir uma meta, gostaria que os elementos selecionados fossem alterados automaticamente para representar 100% da meta.
```

### 2. Estética

```markdown
Na seção Resumão, mude todas as barras que estiverem relacionadas à saída de dinheiro de verde para a cor que está sendo utilizada para representar as Despesas.
```

```markdown
Faça o mesmo (alterar as barras selecionadas para `bg-clay') na seção Despesas por categoria.
```

### 3. Página Resumo

```markdown
Na página `/resumo`, crie uma seção "Receitas por categoria". Mantenha as barras verdes neste caso.
```

### 4. Página Relatórios

```markdown
Em `/relatorios`, ao invés de mostrar apenas um gráfico de Receitas e despesas por mês, coloque um filtro de data para alterar a visualização de acordo com o período desejado.
```
