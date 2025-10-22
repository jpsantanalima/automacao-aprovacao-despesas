# 💼 Automação de Aprovação de Despesas com Power Automate

Este projeto utiliza o Microsoft Power Automate para automatizar o processo de aprovação de despesas por setor, com base em dados estruturados em uma planilha Excel.

## 📊 Objetivo

Agilizar o controle financeiro e garantir que os gastos de cada setor estejam dentro dos limites orçamentários definidos, com envio automático de notificações por e-mail.

## 🧠 Como funciona

1. Leitura da planilha Excel com três abas:
   - `Custos`: colaboradores e setores.
   - `Base`: despesas realizadas por setor.
   - `LimiteCustos`: limite mensal e margem de tolerância por setor.

2. Processamento dos dados:
   - Soma das despesas por setor.
   - Cálculo do limite ajustado com margem.
   - Verificação se o total de despesas ultrapassa o limite permitido.

3. Decisão automatizada:
   - Se as despesas estiverem dentro do limite, o setor recebe um e-mail de aprovação.
   - Se ultrapassarem, o setor recebe um e-mail de reprovação com os detalhes.

## 📂 Estrutura do fluxo

- Gatilho: Quando um novo e-mail chega com a planilha anexada.
- Ações:
  - Leitura das tabelas.
  - Aplicação de lógica condicional.
  - Criação de tabela HTML com os dados.
  - Envio de e-mail com formatação CSS.

## 📧 Notificações

Os e-mails enviados incluem:
- Nome do setor.
- Total de despesas.
- Limite permitido.
- Status da aprovação (✅ ou ❌).

## 🛠️ Requisitos

- Conta Microsoft com acesso ao Power Automate.
- Conexões ativas com Outlook e Excel Online.
- Permissão para leitura de arquivos do OneDrive ou SharePoint.

