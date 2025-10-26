# 🚀 Designer-in-Dev-Mode: Mentoria Frontend para Designers

Este repositório é o *hub* central da nossa jornada de mentoria, focada em transformar a visão de design em código funcional, limpo e profissional. O objetivo é colocar o designer em "modo desenvolvedor".

**O objetivo principal é traduzir o conhecimento de design em uma compreensão do fluxo de trabalho de desenvolvimento, desde a organização do código (Git/VS Code) até a implementação com HTML, CSS, JavaScript e o framework Angular.**

## 💡 Por que esta mentoria?

Como designer, você já domina os princípios visuais e de experiência do usuário. Agora, vamos dar o próximo passo: entender como suas criações ganham vida no código. Esta mentoria foi especialmente desenvolvida para:

- 🎨 Traduzir conceitos de design para código
- 🛠️ Dominar ferramentas essenciais do desenvolvimento
- 🤖 Aproveitar o poder da IA no fluxo de trabalho
- 🔄 Compreender o ciclo do desenvolvimento frontend

---

## 🎯 Projeto Hands-on: Landing Page (LP) Simples

Todas as nossas sessões práticas serão aplicadas no desenvolvimento de uma Landing Page (LP) simples, que será prototipada por você e implementada por nós, passo a passo.

---

## 📅 Cronograma da Mentoria (Encontros Quinzenais - 1h)

| Encontro | Tema Principal | Tópicos de Foco | Foco Prático | Pasta de Trabalho |
| :---: | :--- | :--- | :--- | :---: |
| **1** | **Fundamentos da Produtividade: VS Code & GitHub** | **VS Code:** Configuração, Atalhos, Extensões Essenciais (*Live Server*, *Prettier*). **GitHub:** Conceitos de Git, Fluxo `commit`, `branch`, `PR` (Pull Request). | Configurar o ambiente. Criar o repositório. **Tarefa:** Desenhar o protótipo da LP. | `01-encontro-vscode-github` |
| **2** | **IA, HTML Semântico e Estrutura** | **IA:** GitHub Copilot (geração de código via comentários) e outras ferramentas. **HTML Semântico:** Tags estruturais (`header`, `main`, `section`). **Acessibilidade:** Atributo `alt` em imagens. | **Hands-on:** Usar IA para gerar um bloco. Criar a estrutura HTML da LP. | `02-encontro-ia-html` |
| **3** | **Layout e Design Responsivo (CSS/Flexbox)** | **CSS Básico e Box Model:** `margin`, `padding`, `border` (tradução do espaçamento de design). **Flexbox:** Eixos, alinhamentos. **Responsividade:** Media Queries. | Aplicar estilos. Criar o *Header* e a seção de *Features* da LP usando **Flexbox**. | `03-encontro-layout-responsivo` |
| **4** | **JavaScript e Interatividade** | **JavaScript Essencial:** Variáveis, Funções, Manipulação do DOM. **Eventos:** Adicionar um evento de *click* (ex: menu *mobile*). **Interação:** Tradução de estados de design para o JS. | Implementar um menu hamburguer interativo ou um *modal* na LP, usando JS puro. | `04-encontro-javascript` |
| **5** | **Introdução ao Angular e Componentização** | **Por que Frameworks?** O problema da escala. **Conceito de Componente:** Componente Angular = Componente do Design System. **Estrutura:** Templates, Estilos Isolados. **Data Binding:** O conceito de *Input* (dados que o componente recebe). | Criar um projeto Angular simples. Isolar a seção de *Features* da LP em um componente Angular. | `05-encontro-angular-component` |
| **6** | **Design System & Performance** | **Tokens de Design:** CSS Variables, SASS. **IDS:** Utilização do IDS **Deploy:** GitHub Pages, Vercel. | Implementar design system, otimizar performance e realizar deploy. | `06-encontro-deploy` |
| **7** | **Projeto Final & Code Review** | **Code Review:** Boas práticas, Clean Code. **Git:** Resolução de conflitos, Git Flow. **CI/CD:** GitHub Actions básico. | Finalizar o projeto, realizar code review e configurar pipeline de deploy automático. | `07-encontro-final` |

---

## 🛠️ Fluxo de Trabalho e Regras de Colaboração (O Processo Profissional)

O aprendizado com Git/GitHub é central. Você deve seguir este fluxo para cada atividade:

### 1. **Fork do Repositório (Apenas 1 Vez)**
Faça uma cópia deste repositório para a sua conta pessoal.

### 2. **Configuração do Ambiente**
```bash
# Clone seu fork
git clone https://github.com/SEU-USERNAME/designer-in-dev-mode.git

# Entre no diretório
cd designer-in-dev-mode

# Instale as dependências (quando necessário)
npm install
```

### 3. **Fluxo de Trabalho por Encontro**
```bash
# Atualize seu fork com o repositório principal
git pull upstream main

# Crie uma branch para o encontro
git switch -c feature/encontro-X-descricao

# Faça commits frequentes
git add .
git commit -m "feat: adiciona estrutura inicial do header"

# Envie as alterações
git push origin feature/encontro-X-descricao
```

### 4. **Pull Request**
- Abra um PR do seu fork para o repositório principal
- Aguarde o code review
- Faça as alterações solicitadas, se necessário
- Merge após aprovação

## 📚 Recursos Adicionais

- [VS Code para Designers](https://code.visualstudio.com/docs/editor/accessibility)
- [Git & GitHub para Designers](https://www.atlassian.com/git/tutorials/what-is-version-control)
- [Angular Documentation](https://angular.io/docs)
- [MDN Web Docs](https://developer.mozilla.org/pt-BR/)
- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)

## 🤝 Combinados

- Faça perguntas! Não existe pergunta ruim
- Compartilhe seus conhecimentos de design
- Pratique regularmente entre as sessões
- Comunique qualquer dificuldade ou dúvida

Happy coding! 🎨💻
