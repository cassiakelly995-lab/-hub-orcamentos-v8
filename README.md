# 📋 Painel Integrado de Orçamentos — OAB Santana de Parnaíba

> Sistema web para gestão de orçamentos, fornecedores e compras da subseção da OAB de Santana de Parnaíba. Roda direto no navegador, sincroniza em tempo real entre dispositivos e não exige instalação.

![Status](https://img.shields.io/badge/status-ativo-brightgreen)
![Firebase](https://img.shields.io/badge/Firebase-Realtime%20DB-orange?logo=firebase)
![Feito com](https://img.shields.io/badge/feito%20com-HTML%20%2B%20JS%20puro-blue)

---

## 🏛️ Sobre o Projeto

Desenvolvido para a equipe administrativa da OAB Santana de Parnaíba, o painel centraliza três processos que antes dependiam de planilhas espalhadas e e-mails confusos: **cotações de serviços, cadastro de fornecedores e listas de compras colaborativas**.

Qualquer pessoa da equipe consegue usar no primeiro acesso, sem treinamento técnico, tanto no celular quanto no computador.

---

## ✨ O que o sistema faz

### 📄 Orçamentos para Sites
- Registra propostas de fornecedores com valor, prazo e condições de pagamento
- Compara automaticamente as propostas e destaca o menor preço
- Gera relatório PDF formal com parecer técnico e área de assinatura

### 🏢 Gestão de Fornecedores
- Cadastro completo com categoria, avaliação por estrelas e histórico
- Filtros por segmento para localizar fornecedores rapidamente

### 🛒 Compras Gimba — fluxo colaborativo
- A responsável preenche o estoque atual e os produtos necessários
- Envia um link direto para a chefe revisar e aprovar
- A chefe preenche as quantidades a comprar e aprova — tudo no mesmo sistema
- Fluxo de status claro: `Preenchido → Aguardando Chefia → Aprovado → Finalizado`
- Exportação em PDF com campos de assinatura para arquivo físico

---

## 🛠️ Tecnologias

- **HTML, CSS e JavaScript puro** — sem frameworks, leve e rápido
- **Firebase Realtime Database** — dados sincronizados em tempo real entre dispositivos
- Funciona em qualquer hospedagem estática

---

## 🗺️ Próximas melhorias

- [ ] Login com autenticação para restringir acesso
- [ ] Notificação automática para a chefe quando uma lista precisar de aprovação
- [ ] Gráficos de gastos por período
- [ ] Histórico de edições com registro de quem alterou e quando
- [ ] Modo escuro
- [ ] Versão instalável no celular (PWA)

---

<p align="center">
  Desenvolvido com 💛 para a equipe da OAB Santana de Parnaíba
</p>
