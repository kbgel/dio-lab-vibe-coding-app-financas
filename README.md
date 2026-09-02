# 🌅 Alvorada — Organize suas finanças conversando

[![Acesse o App](https://img.shields.io/badge/🌐_Acessar_o_App-Alvorada-2f5233?style=for-the-badge)](https://alvorada-fin.lovable.app/)
[![Feito com Lovable](https://img.shields.io/badge/Feito_com-Lovable-ff6b6b?style=for-the-badge)](https://lovable.dev)
[![Desafio DIO](https://img.shields.io/badge/Desafio-DIO-purple?style=for-the-badge)](https://dio.me)

> **Desafio de Projeto — DIO**  
> Criando um App de Organização de Finanças Pessoais com IA · Vibe Coding

---

## 📋 Sobre o Projeto

O **Alvorada** é um conceito de aplicativo de finanças pessoais que coloca a **conversa** como interface principal. Em vez de formulários, planilhas ou menus complexos, o usuário registra gastos e receitas escrevendo como falaria com alguém:

> *"Gastei R$ 42,90 no mercado hoje"*  
> *"Recebi R$ 2.500 de salário ontem"*  
> *"Depositar R$ 100 na reserva de emergência"*

O app interpreta a mensagem, mostra o que entendeu e só salva depois da confirmação do usuário. Tudo com um tom educativo, sem julgamento e com transparência sobre o que é sugestão da IA.

### ✨ Principais funcionalidades

| Funcionalidade | Descrição |
|---|---|
| **💬 Conversa** | Registre receitas, despesas e interaja com metas em linguagem natural |
| **📊 Resumo** | Visão geral de saldo, receitas, despesas e categorias do período |
| **📃 Transações** | Lista pesquisável e filtrável de todas as movimentações |
| **🎯 Metas** | Crie, acompanhe e gerencie metas financeiras com depósitos e saques |
| **📈 Relatórios** | Gráficos de evolução com filtro de data personalizável |
| **🏷️ Categorias** | Organize suas transações em categorias editáveis |
| **⚙️ Ajustes** | Preferências de acessibilidade, exportação CSV e configurações gerais |
| **❓ Ajuda** | Exemplos de uso e orientações sobre o app |

### 🎨 Identidade visual

O Alvorada adota uma paleta de cores naturais e acolhedoras:

- **Sage (verde-sálvia)** para receitas e elementos positivos
- **Clay (terracota)** para despesas e alertas
- **Cream e Sand** como base, criando um visual leve e convidativo
- Tipografia: **Manrope** (interface) e **Fraunces** (títulos)

### ♿ Design Universal

O projeto foi construído com **Design Universal** como requisito, não como retoque final:

- Navegação por teclado com foco visível
- Compatibilidade com leitores de tela (rótulos ARIA, `sr-only`, `aria-live`)
- Contraste adequado e informação que não depende só de cor
- Alvos de toque amplos (mín. 44px)
- Respeito a `prefers-reduced-motion` e `prefers-contrast: high`
- Responsivo: funciona em celular, tablet e desktop

---

## 🛠️ Tecnologias e Ferramentas

| Ferramenta | Uso |
|---|---|
| **Copilot** | Revisão e refinamento do PRD (Product Requirements Document) |
| **Lovable** | Geração do MVP funcional a partir do PRD via Vibe Coding |
| **Vibe Coding** | Abordagem criativa de programar guiando a IA com prompts claros |

---

## 🤖 Prompt Final (PRD)

O processo de criação seguiu estas etapas:

1. **Rascunho inicial** — Foi criado um PRD curto com contexto, problema, público-alvo e funcionalidades-chave
2. **Revisão com Copilot** — Pedi ao Copilot que refinasse o PRD, gerando um documento completo com 21 seções
3. **Geração no Lovable** — Usei o PRD revisado como input direto no Lovable
4. **Ajustes iterativos** — Fiz refinamentos pontuais via prompts curtos no Lovable

### 📂 Onde encontrar

Todas as interações estão documentadas na pasta [`prompts/`](prompts/):

| Arquivo | Conteúdo |
|---|---|
| [`interacoes-ias.md`](prompts/interacoes-ias.md) | Resumo organizado: prompt inicial, visão geral do PRD e ajustes feitos no Lovable |
| [`prd-revisado.md`](prompts/prd-revisado.md) | Arquivo completo com o PRD na íntegra (21 seções, ~400 linhas) |

---

## 🔮 Melhorias Futuras

Por conta dos limites de créditos da versão gratuita do Lovable, não foi possível iterar tanto quanto desejado. Abaixo estão melhorias que enriqueceriam o app:

### Interface e Experiência

- [ ] **Modo escuro** — Implementar alternância entre tema claro e escuro, respeitando `prefers-color-scheme`
- [ ] **Onboarding guiado** — Tela de boas-vindas para primeiro acesso com configuração progressiva (nome, moeda, renda mensal)
- [ ] **Notificações e lembretes** — Lembretes configuráveis para registrar gastos e acompanhar metas
- [ ] **Feedback visual nas ações** — Micro-animações de confirmação ao salvar, editar ou excluir registros (toasts, transições)

### Agente Financeiro

- [ ] **Dicas contextualizadas** — O agente sugere economias baseadas em padrões reais do histórico do usuário, não apenas dicas genéricas
- [ ] **Consultas complexas** — Suporte a perguntas como "quanto gastei em alimentação nos últimos 3 meses?" ou "comparar despesas de julho e agosto"
- [ ] **Detecção de recorrências** — Identificar gastos recorrentes automaticamente e sugerir cadastrá-los como fixos
- [ ] **Entrada por voz** — Permitir registro de transações por voz, com transcrição e confirmação

### Dados e Relatórios

- [ ] **Gráficos comparativos** — Comparação lado a lado entre períodos (ex: este mês vs. mês passado)
- [ ] **Relatório de metas** — Histórico de depósitos/saques em cada meta, com projeção de conclusão
- [ ] **Exportação em PDF** — Além do CSV, gerar relatórios visuais exportáveis
- [ ] **Persistência real** — Migrar do `localStorage` para banco de dados com autenticação, permitindo acesso em múltiplos dispositivos

### Acessibilidade e Inclusão

- [ ] **Alto contraste aprimorado** — Tema de alto contraste dedicado, além do suporte básico via `prefers-contrast`
- [ ] **Atalhos de teclado** — Atalhos para ações frequentes (ex: `Ctrl+N` para nova transação, `Ctrl+/` para focar no chat)

---

## 💭 Reflexão

Este desafio me mostrou que o **Vibe Coding** é muito mais do que "pedir para a IA programar". É um exercício de **comunicação clara e pensamento de produto**.

### O que aprendi

- **A qualidade do prompt define a qualidade do resultado.** Quanto mais estruturado e específico o PRD, melhor o MVP gerado pelo Lovable. Detalhes como tom de voz, estados de erro e princípios de acessibilidade fizeram diferença real no output.

- **Iterar é essencial.** A primeira versão nunca é a final. Os ajustes que fiz no Lovable (metas pelo chat, cores das barras, filtro de data nos relatórios) mostraram como refinamentos pequenos melhoram muito a experiência.

- **Design Universal não é "extra".** Incluir acessibilidade desde o PRD, e não como correção posterior, resultou em um app que já nasceu com navegação por teclado, suporte a leitores de tela e alvos de toque amplos.

- **A IA é uma parceira, não uma substituta.** O Copilot me ajudou a organizar e expandir o PRD, e o Lovable transformou o documento em telas funcionais. Mas as decisões de produto, os ajustes de UX e o olhar crítico continuam sendo humanos.

### O que faria diferente

Com maiores limites de crédito no Lovable, investiria em modo escuro, onboarding guiado e dicas mais inteligentes do agente. Também testaria o app com pessoas reais para validar se a experiência conversacional é tão intuitiva quanto parece no protótipo.

---

## 🔗 Links

| Recurso | Link |
|---|---|
| 🌐 App (demo) | [alvorada-fin.lovable.app](https://alvorada-fin.lovable.app/) |
| 📦 Repositório base (DIO) | [dio-lab-vibe-coding-app-financas](https://github.com/digitalinnovationone/dio-lab-vibe-coding-app-financas) |
