# 📋 Painel Integrado de Orçamentos — OAB Santana de Parnaíba

> Sistema web completo para gestão de orçamentos, fornecedores e compras da subseção da OAB de Santana de Parnaíba — construído com HTML puro e Firebase Realtime Database, sem frameworks ou dependências pesadas.

![Status](https://img.shields.io/badge/status-ativo-brightgreen)
![Firebase](https://img.shields.io/badge/Firebase-Realtime%20DB-orange?logo=firebase)
![Licença](https://img.shields.io/badge/licença-privado-lightgrey)
![Feito com](https://img.shields.io/badge/feito%20com-HTML%20%2B%20JS%20puro-blue)

---

## 🏛️ Sobre o Projeto

Este painel foi desenvolvido para resolver um problema real e cotidiano da equipe administrativa da OAB Santana de Parnaíba: **organizar cotações, fornecedores e listas de compras de forma colaborativa e sem papelada**.

O sistema roda direto no navegador — sem instalação, sem servidor próprio — e sincroniza os dados em tempo real entre todos os dispositivos via Firebase.

---

## ✨ Funcionalidades

### 📄 Orçamentos para Sites
- Registro de propostas de fornecedores com todos os campos relevantes (valor, prazo, condições)
- **Comparativo automático** de preços com destaque para o menor valor
- Geração de **relatório PDF formal** com parecer técnico e área de assinatura
- Filtros por status (pendente, aprovado, reprovado) e busca em tempo real
- CRUD completo com sincronização instantânea no Firebase

### 🏢 Gestão de Fornecedores
- Cadastro com categoria, avaliação por estrelas, contato e histórico
- Cards visuais com filtros por segmento
- Edição e exclusão direto do card

### 🛒 Compras Gimba (fluxo colaborativo)
- Cássia preenche o estoque atual e os produtos necessários
- Salva e envia um **link único para a chefe aprovar**
- A chefe acessa o mesmo painel, preenche a coluna de quantidade a comprar (destacada em dourado)
- Fluxo de status: `Cássia preencheu → Aguardando Chefia → Aprovado → Finalizado`
- Exportação em PDF com campos de assinatura

---

## 🖼️ Screenshots

> _Adicione aqui capturas de tela das três abas do painel: Orçamentos, Fornecedores e Compras Gimba._

| Orçamentos | Fornecedores | Compras Gimba |
|:-----------:|:------------:|:-------------:|
| _(imagem)_ | _(imagem)_   | _(imagem)_    |

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Uso |
|---|---|
| **HTML5 + CSS3 + JavaScript** | Interface e lógica completa, sem frameworks |
| **Firebase Realtime Database** | Persistência e sincronização em tempo real |
| **Firebase SDK v10** (via CDN) | Integração com o banco — importado como módulo ES |
| **Google Fonts** | Playfair Display + DM Sans + DM Mono |
| **Print CSS** | Geração de PDF diretamente pelo navegador |

> Nenhum bundler, nenhum Node.js, nenhuma dependência local. Funciona em qualquer hospedagem estática ou até aberto como arquivo local.

---

## 🚀 Como Usar

### Pré-requisitos
- Conta no [Firebase](https://firebase.google.com/) com um projeto criado
- Realtime Database habilitado no projeto Firebase

### Passo a passo

1. **Clone ou baixe o repositório**
   ```bash
   git clone https://github.com/seu-usuario/oab-santana-painel.git
   ```

2. **Configure o Firebase**

   Abra o arquivo `index.html` e substitua o objeto `_cfg` pelas credenciais do seu projeto Firebase:
   ```js
   const _cfg = {
     apiKey: "SUA_API_KEY",
     authDomain: "seu-projeto.firebaseapp.com",
     databaseURL: "https://seu-projeto-default-rtdb.firebaseio.com",
     projectId: "seu-projeto",
     storageBucket: "seu-projeto.appspot.com",
     messagingSenderId: "000000000000",
     appId: "1:000000000000:web:xxxxxxxxxxxxxxxx"
   };
   ```

3. **Configure as regras do Realtime Database**

   No console do Firebase, vá em _Realtime Database → Regras_ e defina:
   ```json
   {
     "rules": {
       ".read": true,
       ".write": true
     }
   }
   ```
   > ⚠️ Em produção, restrinja o acesso com autenticação Firebase.

4. **Abra o arquivo**

   Basta abrir o `index.html` no navegador — ou subir para qualquer hospedagem estática (GitHub Pages, Netlify, Firebase Hosting etc.).

---

## 🗺️ Roadmap

- [ ] Autenticação por e-mail (Firebase Auth) para restringir acesso
- [ ] Notificação por e-mail quando a chefe precisar aprovar uma lista
- [ ] Dashboard com gráficos de gastos por período
- [ ] Histórico de alterações com registro de quem editou e quando
- [ ] Modo escuro
- [ ] PWA — instalável no celular como aplicativo

---

## 🤝 Contexto e Motivação

Este projeto nasceu de uma necessidade prática: a equipe da OAB precisava de uma forma simples e confiável de registrar cotações sem depender de planilhas espalhadas, e-mails confusos ou processos manuais. A proposta foi criar algo que **qualquer pessoa da equipe consiga usar no primeiro acesso**, sem treinamento técnico — e que funcione igualmente bem no celular ou no computador.

---

## 📄 Licença

Uso interno — OAB Santana de Parnaíba. Adaptações para outras subseções são bem-vindas mediante crédito ao projeto original.

---

<p align="center">
  Desenvolvido com 💛 para a equipe da OAB Santana de Parnaíba
</p>
