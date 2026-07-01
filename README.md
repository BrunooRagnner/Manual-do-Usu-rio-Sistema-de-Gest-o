# Manual-do-Usu-rio-Sistema-de-Gest-o
📘 MANUAL DO USUÁRIO – SISTEMA DE GESTÃO UNIVERSAL Apresentação O Sistema de Gestão Universal é uma plataforma completa desenvolvida para otimizar o dia a dia de comércios, prestadores de serviços e pequenas empresas








# 🚀 Sistema de Gestão Universal

Sistema completo para gestão de comércio, serviços e estoque, com foco em **PDV (Ponto de Venda)**, **controle de caixa**, **fiados**, **estoque inteligente**, **fidelidade** e **análise de dados** – tudo em uma única plataforma.

---

## 📖 Sobre o Projeto

O **Sistema de Gestão Universal** foi desenvolvido para atender pequenos e médios negócios (conveniências, padarias, lojas de varejo, prestadores de serviço) que precisam de um sistema unificado para:

- Realizar vendas no PDV com suporte a múltiplas formas de pagamento, split de pagamento e venda fiada.
- Controlar o caixa (abertura, fechamento, suplementos, sangrias, histórico).
- Gerenciar estoque com análises inteligentes (previsão de consumo, sugestão de compra, curva ABC).
- Administrar clientes, fornecedores e funcionários.
- Registrar e cobrar clientes com saldo devedor (fiados).
- Gerenciar entregas, lotes, transferências e inventário.
- Oferecer programa de fidelidade com níveis (Bronze, Prata, Ouro).
- Gerar relatórios financeiros e de estoque em PDF.
- Utilizar um assistente IA para previsões e alertas.

O sistema foi projetado para ser **100% offline** no PDV (com sincronização automática quando a conexão retorna) e **multi-usuário** com permissões granulares (vendedor, caixa, gerente, administrador).

---

## ✨ Principais Funcionalidades

### 🛒 PDV (Ponto de Venda)
- Busca rápida por nome ou código de barras.
- Carrinho de compras com ajuste de quantidade.
- Aplicação de descontos (percentual ou fixo).
- Split de pagamento (divide a venda em múltiplas formas).
- Atalhos pelo teclado (F1 a F4 para formas de pagamento, F9 finalizar, F12 reimprimir).
- Impressão de cupom via Bluetooth (impressora térmica) ou PDF.
- Modo offline: vendas são salvas localmente e sincronizadas automaticamente.

### 💰 Caixa
- Abertura com valor inicial.
- Suplementos e sangrias com registro de motivo.
- Fechamento com contagem de dinheiro físico e cálculo de diferença.
- Histórico completo de todos os períodos.

### 📦 Itens
- Cadastro, edição e exclusão de produtos/serviços.
- Atributos: código, categoria, unidade, estoque, preço, impostos (ICMS, IPI, PIS, COFINS).
- Upload de imagens.
- Sugestão de preço com IA baseada em margem, categoria e estoque.
- Curva ABC (classificação de itens por importância).

### 👥 Pessoas
- Cadastro de clientes, fornecedores e funcionários.
- Controle de limite de crédito e saldo (fiados).
- Pontos de fidelidade automáticos.

### 📄 Transações
- Histórico detalhado de vendas e pagamentos.
- Filtros por data, cliente, tipo e forma de pagamento.
- Emissão de comprovante (PDF).

### 🚚 Entregas
- Criação de pedidos de entrega com endereço e taxa.
- Atualização de status (pendente, em andamento, concluída, cancelada).

### 👑 Fidelidade
- Configuração de pontos por real gasto.
- Níveis: Bronze (5% desconto), Prata (5%), Ouro (10%).
- Ranking dos clientes com mais pontos.

### 📊 Estoque
- Resumo com total de itens, valor, itens críticos e giro estimado.
- Análise detalhada por item: consumo (30d), previsão (7d), dias de cobertura, sugestão de compra, prioridade.
- Filtros por status (crítico, zerado, normal).
- Exportação para PDF.

### 🤝 Fiados
- Lista de clientes devedores com saldo e dias de atraso.
- Ações por cliente: cobrança via WhatsApp/SMS, ligação, pagamento, quitação, recibo detalhado, link de pagamento, agendamento de lembrete.

### 🔄 Lotes, Transferências e Inventário
- Controle de lotes por validade, fornecedor e nota fiscal.
- Transferência de itens entre armazéns.
- Inventário físico com ajuste automático de estoque.

### 🤖 Assistente IA
- Chat interativo com comandos:
  - `previsão` – previsão de vendas para 7 dias.
  - `compra` – sugestões de reposição de estoque.
  - `fluxo` – alerta de fluxo de caixa.
  - `estoque` – produtos críticos.
  - `ajuda` – lista de comandos.

### 📈 Gestor (painel do proprietário)
- Visão geral do caixa (aberto/fechado, saldos, vendas do dia).
- Resumo diário (total de vendas, ticket médio, clientes, produtos vendidos).
- Estoque com análise inteligente.
- Lista de fiados.
- Gráfico de vendas por hora.
- Atualizações em tempo real via WebSocket.

### 🔐 Administração
- Gerenciamento de usuários e permissões.
- Cadastro de novas licenças.
- Logs de auditoria.
- Backup/restore (exportação/importação JSON).

---

## 🛠️ Tecnologias Utilizadas

### Backend
- **FastAPI** – Framework Python para APIs REST.
- **SQLAlchemy** – ORM para banco de dados (SQLite/PostgreSQL).
- **JWT** – Autenticação segura.
- **WebSocket** – Comunicação em tempo real.
- **ReportLab** – Geração de PDFs.
- **Prometheus** – Métricas e monitoramento.
- **APScheduler** – Agendamento de tarefas.
- **bcrypt** – Hash de senhas.

### Frontend
- **Vue 3** – Framework progressivo para UI.
- **Vite** – Build tool rápido.
- **Chart.js** – Gráficos interativos.
- **jsPDF** – Geração de PDF no navegador.
- **Axios** – Cliente HTTP.

### Infraestrutura
- **Docker** – Containerização e facilidade de deploy.
- **Cloudflare Tunnel** – Exposição segura (opcional).
- **ngrok** – Túneis para testes (opcional).

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
- Python 3.10+
- Node.js 16+
- pip e npm
- (Opcional) Docker e Docker Compose

### 1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/sistema-gestao.git
cd sistema-gestao
