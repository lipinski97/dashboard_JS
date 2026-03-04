# 🏗️ Dashboard de Gestão de Prazos de Obra

![Status do Projeto](https://img.shields.io/badge/status-ativo-brightgreen)
![Tecnologia](https://img.shields.io/badge/tecnologia-HTML%20%2B%20CSS%20%2B%20JS-blue)
![License](https://img.shields.io/badge/licen%C3%A7a-MIT-green)

> Dashboard web para gestão e acompanhamento de cronogramas de obras, com leitura direta de arquivos Excel (.xlsx) no navegador — sem necessidade de servidor ou backend.

---

## 🎯 Sobre o Projeto

Este projeto é uma solução prática para **gestores e engenheiros de obras** que precisam visualizar rapidamente o status do cronograma de construção. Com apenas um clique, o usuário importa sua planilha Excel e obtém um painel completo com KPIs, gráficos e alertas de atividades em atraso.

**Desenvolvido como projeto de portfólio** para demonstrar habilidades em:
- Manipulação do DOM com JavaScript puro
- Leitura e parsing de arquivos binários no browser (SheetJS)
- Visualização de dados com Chart.js
- Design responsivo com CSS moderno

---

## ✨ Funcionalidades

| Funcionalidade | Descrição |
|---|---|
| 📂 **Import Excel** | Upload direto de `.xlsx` — processado 100% no navegador |
| 📊 **KPI Cards** | Total, Concluídas, Em Execução, Em Atraso, Não Iniciadas |
| 📅 **Visão Semanal** | Foco operacional: gráficos de atrasos por equipe e motivos |
| 📆 **Visão Mensal** | Foco gerencial: distribuição de tarefas por mês |
| 🔴 **Tabela de Atrasos** | Lista visual de todas as atividades que precisam de atenção |
| 🔍 **Filtro em Tempo Real** | Busca por tarefa, equipe ou motivo na tabela |
| 📱 **Design Responsivo** | Funciona em desktop, tablet e celular |

---

## 🛠️ Tecnologias Utilizadas

- **HTML5** — Estrutura semântica
- **CSS3** — Layout com CSS Grid, Flexbox, Custom Properties (variáveis)
- **JavaScript (ES6+)** — Lógica de negócio, DOM, eventos
- **[SheetJS (xlsx)](https://sheetjs.com/)** — Parsing de arquivos Excel diretamente no browser via `FileReader` API
- **[Chart.js](https://www.chartjs.org/)** — Gráficos interativos (barras horizontais, doughnut, barras empilhadas)

---

## 📁 Estrutura Esperada do Excel

O arquivo `.xlsx` deve conter uma aba com as seguintes colunas:

| Coluna | Descrição |
|---|---|
| `EDT` | Identificador hierárquico da tarefa (ex: 1.0, 2.1, 3.5) |
| `Nome da Tarefa` | Nome da atividade |
| `Início Base` | Data de início planejada |
| `Término Base` | Data de término planejada |
| `Equipe Responsável` | Nome da equipe ou empreiteiro |
| `Execução (%)` | Percentual de conclusão (0–100) |
| `Status Base` | Status atual (CONCLUÍDO, EM EXECUÇÃO, EM ATRASO, NÃO INICIADO) |
| `Status Replan` | Status replanejado |
| `Motivo Atraso` | Motivo do atraso (quando aplicável) |

---

## 🚀 Como Usar

1. **Clone** ou baixe este repositório
2. Abra o arquivo `index.html` no seu navegador
3. Clique em **"Selecionar Arquivo Excel"**
4. Importe o arquivo `.xlsx` com o cronograma da obra
5. O dashboard é gerado automaticamente ✅

> Nenhuma instalação, servidor ou conexão com internet é necessária após o carregamento inicial da página.
