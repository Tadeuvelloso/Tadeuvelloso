# GitHub Profile README Redesign Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Reescrever o README.md do perfil do GitHub para ser atrativo a recrutadores tech, com header animado, tech stack organizado por categoria, stats automáticos do GitHub e seção de contato.

**Architecture:** Arquivo único `README.md` com HTML inline suportado pelo GitHub Markdown. Tech stack usa shields.io badges (tema-agnóstico). Stats usam serviços externos (github-readme-stats, streak-stats). Não há código executável — cada tarefa adiciona uma seção ao README e faz commit.

**Tech Stack:** GitHub Markdown, HTML inline, shields.io, readme-typing-svg, github-readme-stats, streak-stats.demolab.com

---

### Task 1: Header / Hero

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Substituir TODO o conteúdo do README pelo bloco de Header**

Abrir `README.md` e substituir o conteúdo inteiro pelo seguinte:

```markdown
<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&random=false&width=550&lines=Hi+%F0%9F%91%8B+I%27m+Tadeu+Velloso;Fullstack+Developer;React+%7C+Next.js+%7C+Node.js;Open+to+new+opportunities+%E2%9C%85" alt="Typing SVG" />

<br/>

<p>📍 Florianópolis, Brasil &nbsp;&middot;&nbsp; 3+ anos de experiência &nbsp;&middot;&nbsp; Open to opportunities ✅</p>

<br/>

<a href="https://www.linkedin.com/in/YOUR_LINKEDIN_HERE">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
&nbsp;
<a href="mailto:tadeuvellososilva@gmail.com">
  <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
</a>

</div>
```

- [ ] **Step 2: Commit**

```bash
git add README.md
git commit -m "feat: add hero header with typing SVG and contact badges"
```

---

### Task 2: Tech Stack

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Adicionar a seção Tech Stack após o conteúdo existente**

Adicionar ao final do `README.md`:

```markdown

---

## ⚡ Tech Stack

**🎨 Frontend**

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**⚙️ Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)

**🧪 Testes**

![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-45ba4b?style=flat-square&logo=playwright&logoColor=white)

**🗄️ Banco de Dados**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

**🛠️ Ferramentas**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![Slack](https://img.shields.io/badge/Slack-4A154B?style=flat-square&logo=slack&logoColor=white)
```

- [ ] **Step 2: Commit**

```bash
git add README.md
git commit -m "feat: add tech stack section with shields.io badges by category"
```

---

### Task 3: GitHub Stats

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Adicionar a seção de Stats após o Tech Stack**

Adicionar ao final do `README.md` (substituir `Tadeuvelloso` pelo username correto do GitHub se necessário):

```markdown

---

## 📊 GitHub Stats

<div align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=Tadeuvelloso&show_icons=true&theme=transparent&hide_border=true&count_private=true" alt="GitHub Stats" />
  <img height="160" src="https://streak-stats.demolab.com?user=Tadeuvelloso&theme=transparent&hide_border=true" alt="GitHub Streak" />
</div>

<div align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Tadeuvelloso&layout=compact&theme=transparent&hide_border=true" alt="Top Languages" />
</div>
```

> Nota: `theme=transparent` faz os cards se adaptarem automaticamente ao tema claro/escuro do visitante sem necessidade de `<picture>`. Os valores são puxados do GitHub em tempo real.

- [ ] **Step 2: Commit**

```bash
git add README.md
git commit -m "feat: add GitHub stats, streak and top languages cards"
```

---

### Task 4: Seção de Contato

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Adicionar a seção de Contato ao final do README**

Adicionar ao final do `README.md`:

```markdown

---

## 📬 Vamos conversar?

<div align="center">

<p>Estou aberto a novas oportunidades. Sinta-se à vontade para entrar em contato!</p>

<a href="https://www.linkedin.com/in/YOUR_LINKEDIN_HERE">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
&nbsp;
<a href="mailto:tadeuvellososilva@gmail.com">
  <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
</a>

<br/><br/>

<sub>📍 Florianópolis, Brasil 🇧🇷 · Disponível para trabalho remoto</sub>

</div>
```

- [ ] **Step 2: Commit**

```bash
git add README.md
git commit -m "feat: add contact section with LinkedIn and email badges"
```

---

### Task 5: Substituir URL do LinkedIn e fazer push

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Substituir o placeholder do LinkedIn**

No `README.md`, encontrar todas as ocorrências de `YOUR_LINKEDIN_HERE` (aparecem 2 vezes — no header e na seção de contato) e substituir pela URL real do LinkedIn do Tadeu.

Exemplo do resultado esperado:
```
https://www.linkedin.com/in/tadeu-velloso
```
(confirmar o slug exato com o usuário antes de substituir)

- [ ] **Step 2: Commit final**

```bash
git add README.md
git commit -m "feat: replace LinkedIn placeholder with real URL"
```

- [ ] **Step 3: Push para o GitHub**

```bash
git push origin main
```

- [ ] **Step 4: Verificar no GitHub**

Abrir `https://github.com/Tadeuvelloso` no navegador e confirmar que:
- O typing SVG anima corretamente
- Os badges de contato aparecem no topo
- As categorias de tech stack estão visíveis
- Os cards de stats carregam (pode levar alguns segundos na primeira vez)
- A seção de contato aparece no rodapé
