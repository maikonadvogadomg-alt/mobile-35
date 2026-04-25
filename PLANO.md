# PLANO DO PROJETO: mobile (3)

> Gerado automaticamente pelo SK Code Editor em 25/04/2026, 00:39:23
> **205 arquivo(s)** | **~32.927 linhas de codigo**

---

## RESUMO EXECUTIVO

- **Tipo de aplicacao:** Aplicacao Web Frontend (React)
- **Frontend / Stack principal:** React, TypeScript

**Para rodar o projeto:**
```bash
# Abra index.html no Preview (botao Play)
```

---

## ESTRUTURA DE ARQUIVOS

```
mobile (3)/
├── .sk/
│   ├── diario.md
│   ├── memoria.json
│   └── perfil-jasmim.md
├── api-server/
│   ├── .replit-artifact/
│   │   └── artifact.toml
│   ├── dist/
│   │   ├── thread-stream-worker.mjs
│   │   └── thread-stream-worker.mjs.map
│   ├── src/
│   │   ├── lib/
│   │   │   ├── .gitkeep
│   │   │   └── logger.ts
│   │   ├── middlewares/
│   │   │   └── .gitkeep
│   │   ├── routes/
│   │   │   ├── ai-chat.ts
│   │   │   ├── ai-forward.ts
│   │   │   ├── config.ts
│   │   │   ├── db.ts
│   │   │   ├── drive.ts
│   │   │   ├── exec.ts
│   │   │   ├── github.ts
│   │   │   ├── health.ts
│   │   │   ├── index.ts
│   │   │   ├── legal-ai.ts
│   │   │   ├── proxy.ts
│   │   │   ├── search.ts
│   │   │   ├── twa.ts
│   │   │   ├── upload.ts
│   │   │   ├── voice.ts
│   │   │   └── workspace.ts
│   │   ├── app.ts
│   │   └── index.ts
│   ├── build.mjs
│   ├── package.json
│   ├── pty_helper
│   ├── pty_helper.c
│   └── tsconfig.json
├── code-editor/
│   ├── .replit-artifact/
│   │   └── artifact.toml
│   ├── public/
│   │   ├── favicon.svg
│   │   ├── guia-completo-apk.md
│   │   ├── icon-192.png
│   │   ├── icon-512.png
│   │   ├── manifest.json
│   │   ├── opengraph.jpg
│   │   └── sw.js
│   ├── src/
│   │   ├── components/
│   │   │   ├── ui/
│   │   │   │   ├── accordion.tsx
│   │   │   │   ├── alert-dialog.tsx
│   │   │   │   ├── alert.tsx
│   │   │   │   ├── aspect-ratio.tsx
│   │   │   │   ├── avatar.tsx
│   │   │   │   ├── badge.tsx
│   │   │   │   ├── breadcrumb.tsx
│   │   │   │   ├── button-group.tsx
│   │   │   │   ├── button.tsx
│   │   │   │   ├── calendar.tsx
│   │   │   │   ├── card.tsx
│   │   │   │   ├── carousel.tsx
│   │   │   │   ├── chart.tsx
│   │   │   │   ├── checkbox.tsx
│   │   │   │   ├── collapsible.tsx
│   │   │   │   ├── command.tsx
│   │   │   │   ├── context-menu.tsx
│   │   │   │   ├── dialog.tsx
│   │   │   │   ├── drawer.tsx
│   │   │   │   ├── dropdown-menu.tsx
│   │   │   │   ├── empty.tsx
│   │   │   │   ├── field.tsx
│   │   │   │   ├── form.tsx
│   │   │   │   ├── hover-card.tsx
│   │   │   │   ├── input-group.tsx
│   │   │   │   ├── input-otp.tsx
│   │   │   │   ├── input.tsx
│   │   │   │   ├── item.tsx
│   │   │   │   ├── kbd.tsx
│   │   │   │   ├── label.tsx
│   │   │   │   ├── menubar.tsx
│   │   │   │   ├── navigation-menu.tsx
│   │   │   │   ├── pagination.tsx
│   │   │   │   ├── popover.tsx
│   │   │   │   ├── progress.tsx
│   │   │   │   ├── radio-group.tsx
│   │   │   │   ├── resizable.tsx
│   │   │   │   ├── scroll-area.tsx
│   │   │   │   ├── select.tsx
│   │   │   │   ├── separator.tsx
│   │   │   │   ├── sheet.tsx
│   │   │   │   ├── sidebar.tsx
│   │   │   │   ├── skeleton.tsx
│   │   │   │   ├── slider.tsx
│   │   │   │   ├── sonner.tsx
│   │   │   │   ├── spinner.tsx
│   │   │   │   ├── switch.tsx
│   │   │   │   ├── table.tsx
│   │   │   │   ├── tabs.tsx
│   │   │   │   ├── textarea.tsx
│   │   │   │   ├── toast.tsx
│   │   │   │   ├── toaster.tsx
│   │   │   │   ├── toggle-group.tsx
│   │   │   │   ├── toggle.tsx
│   │   │   │   └── tooltip.tsx
│   │   │   ├── AssistenteJuridico.tsx
│   │   │   ├── CampoLivre.tsx
│   │   │   ├── CodeEditor.tsx
│   │   │   ├── CombinarApps.tsx
│   │   │   ├── DriveBackupPanel.tsx
│   │   │   ├── FileTree.tsx
│   │   │   ├── GitHubPanel.tsx
│   │   │   ├── Manual.tsx
│   │   │   ├── PackageSearch.tsx
│   │   │   ├── Preview.tsx
│   │   │   ├── QuickPrompt.tsx
│   │   │   ├── RealTerminal.tsx
│   │   │   ├── StreamTerminal.tsx
│   │   │   ├── SystemStatusPanel.tsx
│   │   │   ├── TemplateSelector.tsx
│   │   │   ├── Terminal.tsx
│   │   │   ├── VoiceCard.tsx
│   │   │   ├── VoiceMode.tsx
│   │   │   └── WebContainerTerminal.tsx
│   │   ├── hooks/
│   │   │   ├── use-mobile.tsx
│   │   │   └── use-toast.ts
│   │   ├── lib/
│   │   │   ├── ai-service.ts
│   │   │   ├── github-service.ts
│   │   │   ├── projects.ts
│   │   │   ├── store.ts
│   │   │   ├── tts-service.ts
│   │   │   ├── utils.ts
│   │   │   ├── virtual-fs.ts
│   │   │   └── zip-service.ts
│   │   ├── App.tsx
│   │   ├── index.css
│   │   └── main.tsx
│   ├── components.json
│   ├── index.html
│   ├── package.json
│   ├── SYSTEM_DOCS.md
│   ├── tsconfig.json
│   └── vite.config.ts
├── mockup-sandbox/
│   ├── .replit-artifact/
│   │   └── artifact.toml
│   ├── src/
│   │   ├── .generated/
│   │   │   └── mockup-components.ts
│   │   ├── components/
│   │   │   └── ui/
│   │   │       ├── accordion.tsx
│   │   │       ├── alert-dialog.tsx
│   │   │       ├── alert.tsx
│   │   │       ├── aspect-ratio.tsx
│   │   │       ├── avatar.tsx
│   │   │       ├── badge.tsx
│   │   │       ├── breadcrumb.tsx
│   │   │       ├── button-group.tsx
│   │   │       ├── button.tsx
│   │   │       ├── calendar.tsx
│   │   │       ├── card.tsx
│   │   │       ├── carousel.tsx
│   │   │       ├── chart.tsx
│   │   │       ├── checkbox.tsx
│   │   │       ├── collapsible.tsx
│   │   │       ├── command.tsx
│   │   │       ├── context-menu.tsx
│   │   │       ├── dialog.tsx
│   │   │       ├── drawer.tsx
│   │   │       ├── dropdown-menu.tsx
│   │   │       ├── empty.tsx
│   │   │       ├── field.tsx
│   │   │       ├── form.tsx
│   │   │       ├── hover-card.tsx
│   │   │       ├── input-group.tsx
│   │   │       ├── input-otp.tsx
│   │   │       ├── input.tsx
│   │   │       ├── item.tsx
│   │   │       ├── kbd.tsx
│   │   │       ├── label.tsx
│   │   │       ├── menubar.tsx
│   │   │       ├── navigation-menu.tsx
│   │   │       ├── pagination.tsx
│   │   │       ├── popover.tsx
│   │   │       ├── progress.tsx
│   │   │       ├── radio-group.tsx
│   │   │       ├── resizable.tsx
│   │   │       ├── scroll-area.tsx
│   │   │       ├── select.tsx
│   │   │       ├── separator.tsx
│   │   │       ├── sheet.tsx
│   │   │       ├── sidebar.tsx
│   │   │       ├── skeleton.tsx
│   │   │       ├── slider.tsx
│   │   │       ├── sonner.tsx
│   │   │       ├── spinner.tsx
│   │   │       ├── switch.tsx
│   │   │       ├── table.tsx
│   │   │       ├── tabs.tsx
│   │   │       ├── textarea.tsx
│   │   │       ├── toast.tsx
│   │   │       ├── toaster.tsx
│   │   │       ├── toggle-group.tsx
│   │   │       ├── toggle.tsx
│   │   │       └── tooltip.tsx
│   │   ├── hooks/
│   │   │   ├── use-mobile.tsx
│   │   │   └── use-toast.ts
│   │   ├── lib/
│   │   │   └── utils.ts
│   │   ├── App.tsx
│   │   ├── index.css
│   │   └── main.tsx
│   ├── components.json
│   ├── index.html
│   ├── mockupPreviewPlugin.ts
│   ├── package.json
│   ├── tsconfig.json
│   └── vite.config.ts
├── PLANO.md
├── README.md
└── SISTEMA.md
```

---

## STACK TECNOLOGICO DETECTADO

- **Frontend:** React, TypeScript

---

## ROTAS DA API (endpoints detectados automaticamente)

```
USE    /api  (em api-server/src/app.ts)
POST   /ai/chat  (em api-server/src/routes/ai-chat.ts)
POST   /ai/forward  (em api-server/src/routes/ai-forward.ts)
GET    /config  (em api-server/src/routes/config.ts)
POST   /db/neon/create  (em api-server/src/routes/db.ts)
GET    /db/neon/projects  (em api-server/src/routes/db.ts)
POST   /db/neon/credentials  (em api-server/src/routes/db.ts)
POST   /db/execute  (em api-server/src/routes/db.ts)
POST   /db/test-connection  (em api-server/src/routes/db.ts)
GET    /drive/list  (em api-server/src/routes/drive.ts)
POST   /drive/upload  (em api-server/src/routes/drive.ts)
DELETE /drive/delete/:fileId  (em api-server/src/routes/drive.ts)
POST   /exec/npm-install  (em api-server/src/routes/exec.ts)
POST   /exec/run-node  (em api-server/src/routes/exec.ts)
POST   /exec/run-node-vfs  (em api-server/src/routes/exec.ts)
POST   /db/query  (em api-server/src/routes/exec.ts)
POST   /projects/:projectId/exec-stream  (em api-server/src/routes/exec.ts)
GET    /github/user  (em api-server/src/routes/github.ts)
GET    /github/repos  (em api-server/src/routes/github.ts)
POST   /github/repos  (em api-server/src/routes/github.ts)
POST   /github/push  (em api-server/src/routes/github.ts)
DELETE /github/repos/:owner/:repo  (em api-server/src/routes/github.ts)
GET    /healthz  (em api-server/src/routes/health.ts)
USE    /voice  (em api-server/src/routes/index.ts)
POST   /legal/process  (em api-server/src/routes/legal-ai.ts)
POST   /legal/refine  (em api-server/src/routes/legal-ai.ts)
GET    /search  (em api-server/src/routes/search.ts)
GET    /npm-search  (em api-server/src/routes/search.ts)
GET    /pwa-check  (em api-server/src/routes/twa.ts)
GET    /twa-files  (em api-server/src/routes/twa.ts)
POST   /upload/extract-text  (em api-server/src/routes/upload.ts)
POST   /transcribe  (em api-server/src/routes/voice.ts)
POST   /speak  (em api-server/src/routes/voice.ts)
GET    /workspace/info  (em api-server/src/routes/workspace.ts)
POST   /workspace/write  (em api-server/src/routes/workspace.ts)
GET    /workspace/read  (em api-server/src/routes/workspace.ts)
GET    /workspace/list  (em api-server/src/routes/workspace.ts)
POST   /workspace/delete  (em api-server/src/routes/workspace.ts)
POST   /workspace/install  (em api-server/src/routes/workspace.ts)
POST   /workspace/run  (em api-server/src/routes/workspace.ts)
POST   /workspace/sync  (em api-server/src/routes/workspace.ts)
```

---

## VARIAVEIS DE AMBIENTE NECESSARIAS

Crie um arquivo `.env` na raiz com estas variaveis:

```env
LOG_LEVEL=seu_valor_aqui
DATABASE_URL=seu_valor_aqui
AI_INTEGRATIONS_OPENAI_BASE_URL=seu_valor_aqui
AI_INTEGRATIONS_OPENAI_API_KEY=seu_valor_aqui
PORT=seu_valor_aqui
BASE_PATH=seu_valor_aqui
REPL_ID=seu_valor_aqui
```

---

## ARQUIVOS PRINCIPAIS

- `api-server/src/app.ts` — Ponto de entrada do backend
- `api-server/src/index.ts` — Ponto de entrada do backend
- `api-server/src/routes/index.ts` — Ponto de entrada do backend
- `code-editor/index.html` — Arquivo principal
- `code-editor/src/App.tsx` — Componente raiz do frontend
- `code-editor/src/main.tsx` — Arquivo principal
- `mockup-sandbox/index.html` — Arquivo principal
- `mockup-sandbox/src/App.tsx` — Componente raiz do frontend
- `mockup-sandbox/src/main.tsx` — Arquivo principal

---

## GUIA COMPLETO — O QUE CADA PARTE DO PROJETO FAZ

> Esta secao explica, em linguagem simples, o que e para que serve cada pasta e cada arquivo.

### 📁 Raiz do Projeto (pasta principal)
> Arquivos de configuracao e pontos de entrada ficam aqui.

**`PLANO.md`** _(1393 linhas)_
Este documento! Gerado automaticamente pelo SK Code Editor com toda a estrutura do projeto.

**`README.md`** _(41 linhas)_
Documentacao principal do projeto. Explica o que o projeto faz e como rodar.

**`SISTEMA.md`** _(98 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.sk/`
> Pasta '.sk' — agrupamento de arquivos relacionados.

**`diario.md`** _(11 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`memoria.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`perfil-jasmim.md`** _(36 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `api-server/`
> Pasta 'api-server' — agrupamento de arquivos relacionados.

**`build.mjs`** _(159 linhas)_
Arquivo MJS — parte do projeto.

**`package.json`** _(46 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`pty_helper`** _(16 linhas)_
Arquivo PTY_HELPER — parte do projeto.

**`pty_helper.c`** _(138 linhas)_
Arquivo C — parte do projeto.

**`tsconfig.json`** _(18 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `code-editor/`
> Pasta 'code-editor' — agrupamento de arquivos relacionados.

**`SYSTEM_DOCS.md`** _(292 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`components.json`** _(20 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`index.html`** _(36 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`package.json`** _(93 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(23 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.ts`** _(69 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `mockup-sandbox/`
> Pasta 'mockup-sandbox' — agrupamento de arquivos relacionados.

**`components.json`** _(22 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`index.html`** _(32 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`mockupPreviewPlugin.ts`** _(181 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`package.json`** _(75 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(17 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.ts`** _(73 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `api-server/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(33 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `api-server/dist/`
> Codigo compilado/gerado automaticamente — NAO edite diretamente.

**`thread-stream-worker.mjs`** _(229 linhas)_
Arquivo MJS — parte do projeto.

**`thread-stream-worker.mjs.map`** _(8 linhas)_
Arquivo MAP — parte do projeto.

---

### 📁 `api-server/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`app.ts`** _(35 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(288 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `code-editor/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(32 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `code-editor/public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`favicon.svg`** _(17 linhas)_
Imagem vetorial (icone ou ilustracao que nao perde qualidade ao ampliar).

**`guia-completo-apk.md`** _(949 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`icon-192.png`** _(32 linhas)_
Arquivo de imagem.

**`icon-512.png`** _(100 linhas)_
Arquivo de imagem.

**`manifest.json`** _(61 linhas)_
Manifesto do PWA — define nome, icone e configuracoes para instalar o app no celular.

**`opengraph.jpg`** _(17 linhas)_
Arquivo de imagem.

**`sw.js`** _(121 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `code-editor/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(210 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(167 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(6 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `mockup-sandbox/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(18 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `mockup-sandbox/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(147 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(158 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(6 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `api-server/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`.gitkeep`** _(1 linha)_
Arquivo GITKEEP — parte do projeto.

**`logger.ts`** _(21 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `api-server/src/middlewares/`
> Pasta 'middlewares' — agrupamento de arquivos relacionados.

**`.gitkeep`** _(1 linha)_
Arquivo GITKEEP — parte do projeto.

---

### 📁 `api-server/src/routes/`
> Definicao das URLs e navegacao do app.

**`ai-chat.ts`** _(90 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`ai-forward.ts`** _(156 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`config.ts`** _(27 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`db.ts`** _(362 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`drive.ts`** _(108 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`exec.ts`** _(307 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`github.ts`** _(107 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`health.ts`** _(12 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(37 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`legal-ai.ts`** _(328 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`proxy.ts`** _(62 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`search.ts`** _(63 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`twa.ts`** _(487 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`upload.ts`** _(77 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`voice.ts`** _(88 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`workspace.ts`** _(318 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `code-editor/src/components/`
> Pecas visuais reutilizaveis da interface (botoes, cards, formularios...).

**`AssistenteJuridico.tsx`** _(1286 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`CampoLivre.tsx`** _(740 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`CodeEditor.tsx`** _(154 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`CombinarApps.tsx`** _(277 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`DriveBackupPanel.tsx`** _(200 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`FileTree.tsx`** _(400 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`GitHubPanel.tsx`** _(632 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`Manual.tsx`** _(1655 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`PackageSearch.tsx`** _(415 linhas)_
Componente de BUSCA — campo e logica para filtrar/encontrar conteudo.

**`Preview.tsx`** _(496 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

**`QuickPrompt.tsx`** _(274 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`RealTerminal.tsx`** _(724 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`StreamTerminal.tsx`** _(539 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`SystemStatusPanel.tsx`** _(351 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`TemplateSelector.tsx`** _(501 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`Terminal.tsx`** _(1519 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`VoiceCard.tsx`** _(427 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`VoiceMode.tsx`** _(277 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`WebContainerTerminal.tsx`** _(323 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `code-editor/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`use-toast.ts`** _(192 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de '-toast'.

---

### 📁 `code-editor/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`ai-service.ts`** _(392 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`github-service.ts`** _(197 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`projects.ts`** _(206 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`store.ts`** _(38 linhas)_
STORE de estado — gerencia o estado global do app (dados compartilhados entre telas).

**`tts-service.ts`** _(312 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

**`virtual-fs.ts`** _(200 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`zip-service.ts`** _(163 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

---

### 📁 `mockup-sandbox/src/.generated/`
> Pasta '.generated' — agrupamento de arquivos relacionados.

**`mockup-components.ts`** _(6 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `mockup-sandbox/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`use-toast.ts`** _(190 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de '-toast'.

---

### 📁 `mockup-sandbox/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `code-editor/src/components/ui/`
> Componentes de UI (interface) basicos e genericos.

**`accordion.tsx`** _(56 linhas)_
Componente ACCORDION — secoes que abrem/fecham ao clicar, economizando espaco na tela.

**`alert-dialog.tsx`** _(140 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`alert.tsx`** _(60 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`aspect-ratio.tsx`** _(6 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`avatar.tsx`** _(51 linhas)_
Componente AVATAR — foto ou iniciais do usuario em formato circular.

**`badge.tsx`** _(44 linhas)_
Componente BADGE (etiqueta) — pequeno indicador com numero ou status (ex: '3 novas mensagens').

**`breadcrumb.tsx`** _(116 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`button-group.tsx`** _(84 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`button.tsx`** _(66 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`calendar.tsx`** _(214 linhas)_
Componente CALENDARIO/AGENDA — visualizacao e selecao de datas e eventos.

**`card.tsx`** _(77 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`carousel.tsx`** _(261 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`chart.tsx`** _(368 linhas)_
Componente de GRAFICO — visualizacao de dados em forma de grafico (barras, linhas, pizza...).

**`checkbox.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`collapsible.tsx`** _(12 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`command.tsx`** _(154 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`context-menu.tsx`** _(199 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

**`dialog.tsx`** _(121 linhas)_
Componente DIALOG — caixa de dialogo que exige resposta do usuario (confirmar, cancelar...).

**`drawer.tsx`** _(117 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`dropdown-menu.tsx`** _(202 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`empty.tsx`** _(105 linhas)_
Componente de ESTADO VAZIO — exibido quando nao ha dados para mostrar (ex: 'Nenhum resultado encontrado').

**`field.tsx`** _(245 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`form.tsx`** _(177 linhas)_
Componente de FORMULARIO — campos de entrada de dados (texto, selecao, etc.) com validacao.

**`hover-card.tsx`** _(28 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`input-group.tsx`** _(169 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input-otp.tsx`** _(70 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input.tsx`** _(23 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`item.tsx`** _(194 linhas)_
Componente de ITEM — representa um elemento individual dentro de uma lista ou colecao.

**`kbd.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`label.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`menubar.tsx`** _(255 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`navigation-menu.tsx`** _(129 linhas)_
Componente de NAVEGACAO/CABECALHO — barra superior com logo, menu e links de navegacao.

**`pagination.tsx`** _(118 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`popover.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`progress.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`radio-group.tsx`** _(43 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`resizable.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`scroll-area.tsx`** _(47 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`select.tsx`** _(160 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`separator.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sheet.tsx`** _(141 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sidebar.tsx`** _(728 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`skeleton.tsx`** _(16 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`slider.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sonner.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`spinner.tsx`** _(17 linhas)_
Componente de CARREGAMENTO — animacao visual que aparece enquanto dados estao sendo buscados.

**`switch.tsx`** _(28 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`table.tsx`** _(121 linhas)_
Componente de TABELA — exibe dados em linhas e colunas.

**`tabs.tsx`** _(54 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`textarea.tsx`** _(23 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toast.tsx`** _(128 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toaster.tsx`** _(34 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toggle-group.tsx`** _(62 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toggle.tsx`** _(44 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tooltip.tsx`** _(33 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `mockup-sandbox/src/components/ui/`
> Componentes de UI (interface) basicos e genericos.

**`accordion.tsx`** _(56 linhas)_
Componente ACCORDION — secoes que abrem/fecham ao clicar, economizando espaco na tela.

**`alert-dialog.tsx`** _(140 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`alert.tsx`** _(60 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`aspect-ratio.tsx`** _(6 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`avatar.tsx`** _(51 linhas)_
Componente AVATAR — foto ou iniciais do usuario em formato circular.

**`badge.tsx`** _(38 linhas)_
Componente BADGE (etiqueta) — pequeno indicador com numero ou status (ex: '3 novas mensagens').

**`breadcrumb.tsx`** _(116 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`button-group.tsx`** _(84 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`button.tsx`** _(59 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`calendar.tsx`** _(214 linhas)_
Componente CALENDARIO/AGENDA — visualizacao e selecao de datas e eventos.

**`card.tsx`** _(77 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`carousel.tsx`** _(261 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`chart.tsx`** _(366 linhas)_
Componente de GRAFICO — visualizacao de dados em forma de grafico (barras, linhas, pizza...).

**`checkbox.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`collapsible.tsx`** _(12 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`command.tsx`** _(154 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`context-menu.tsx`** _(199 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

**`dialog.tsx`** _(121 linhas)_
Componente DIALOG — caixa de dialogo que exige resposta do usuario (confirmar, cancelar...).

**`drawer.tsx`** _(117 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`dropdown-menu.tsx`** _(202 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`empty.tsx`** _(105 linhas)_
Componente de ESTADO VAZIO — exibido quando nao ha dados para mostrar (ex: 'Nenhum resultado encontrado').

**`field.tsx`** _(245 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`form.tsx`** _(177 linhas)_
Componente de FORMULARIO — campos de entrada de dados (texto, selecao, etc.) com validacao.

**`hover-card.tsx`** _(28 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`input-group.tsx`** _(166 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input-otp.tsx`** _(70 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input.tsx`** _(23 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`item.tsx`** _(194 linhas)_
Componente de ITEM — representa um elemento individual dentro de uma lista ou colecao.

**`kbd.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`label.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`menubar.tsx`** _(255 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`navigation-menu.tsx`** _(129 linhas)_
Componente de NAVEGACAO/CABECALHO — barra superior com logo, menu e links de navegacao.

**`pagination.tsx`** _(118 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`popover.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`progress.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`radio-group.tsx`** _(43 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`resizable.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`scroll-area.tsx`** _(47 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`select.tsx`** _(160 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`separator.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sheet.tsx`** _(141 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sidebar.tsx`** _(715 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`skeleton.tsx`** _(16 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`slider.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sonner.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`spinner.tsx`** _(17 linhas)_
Componente de CARREGAMENTO — animacao visual que aparece enquanto dados estao sendo buscados.

**`switch.tsx`** _(28 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`table.tsx`** _(121 linhas)_
Componente de TABELA — exibe dados em linhas e colunas.

**`tabs.tsx`** _(54 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`textarea.tsx`** _(23 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toast.tsx`** _(128 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toaster.tsx`** _(34 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toggle-group.tsx`** _(62 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toggle.tsx`** _(44 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tooltip.tsx`** _(33 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

## CONTEXTO PARA IA (copie e cole para continuar o projeto)

> Use este bloco para explicar o projeto para qualquer IA ou desenvolvedor:

```
Projeto: mobile (3)
Tipo: Aplicacao Web Frontend (React)
Stack: React, TypeScript
Arquivos: 205 | Linhas: ~32.927
Rotas API: 41 endpoint(s) detectado(s)
Variaveis de ambiente necessarias: LOG_LEVEL, DATABASE_URL, AI_INTEGRATIONS_OPENAI_BASE_URL, AI_INTEGRATIONS_OPENAI_API_KEY, PORT, BASE_PATH, REPL_ID

Estrutura principal:
  .sk/diario.md
  .sk/memoria.json
  .sk/perfil-jasmim.md
  PLANO.md
  README.md
  SISTEMA.md
  api-server/.replit-artifact/artifact.toml
  api-server/build.mjs
  api-server/dist/thread-stream-worker.mjs
  api-server/dist/thread-stream-worker.mjs.map
  api-server/package.json
  api-server/pty_helper
  api-server/pty_helper.c
  api-server/src/app.ts
  api-server/src/index.ts
  api-server/src/lib/.gitkeep
  api-server/src/lib/logger.ts
  api-server/src/middlewares/.gitkeep
  api-server/src/routes/ai-chat.ts
  api-server/src/routes/ai-forward.ts
  api-server/src/routes/config.ts
  api-server/src/routes/db.ts
  api-server/src/routes/drive.ts
  api-server/src/routes/exec.ts
  api-server/src/routes/github.ts
  api-server/src/routes/health.ts
  api-server/src/routes/index.ts
  api-server/src/routes/legal-ai.ts
  api-server/src/routes/proxy.ts
  api-server/src/routes/search.ts
  api-server/src/routes/twa.ts
  api-server/src/routes/upload.ts
  api-server/src/routes/voice.ts
  api-server/src/routes/workspace.ts
  api-server/tsconfig.json
  code-editor/.replit-artifact/artifact.toml
  code-editor/SYSTEM_DOCS.md
  code-editor/components.json
  code-editor/index.html
  code-editor/package.json
  code-editor/public/favicon.svg
  code-editor/public/guia-completo-apk.md
  code-editor/public/icon-192.png
  code-editor/public/icon-512.png
  code-editor/public/manifest.json
  code-editor/public/opengraph.jpg
  code-editor/public/sw.js
  code-editor/src/App.tsx
  code-editor/src/components/AssistenteJuridico.tsx
  code-editor/src/components/CampoLivre.tsx
  code-editor/src/components/CodeEditor.tsx
  code-editor/src/components/CombinarApps.tsx
  code-editor/src/components/DriveBackupPanel.tsx
  code-editor/src/components/FileTree.tsx
  code-editor/src/components/GitHubPanel.tsx
  code-editor/src/components/Manual.tsx
  code-editor/src/components/PackageSearch.tsx
  code-editor/src/components/Preview.tsx
  code-editor/src/components/QuickPrompt.tsx
  code-editor/src/components/RealTerminal.tsx
  code-editor/src/components/StreamTerminal.tsx
  code-editor/src/components/SystemStatusPanel.tsx
  code-editor/src/components/TemplateSelector.tsx
  code-editor/src/components/Terminal.tsx
  code-editor/src/components/VoiceCard.tsx
  code-editor/src/components/VoiceMode.tsx
  code-editor/src/components/WebContainerTerminal.tsx
  code-editor/src/components/ui/accordion.tsx
  code-editor/src/components/ui/alert-dialog.tsx
  code-editor/src/components/ui/alert.tsx
  code-editor/src/components/ui/aspect-ratio.tsx
  code-editor/src/components/ui/avatar.tsx
  code-editor/src/components/ui/badge.tsx
  code-editor/src/components/ui/breadcrumb.tsx
  code-editor/src/components/ui/button-group.tsx
  code-editor/src/components/ui/button.tsx
  code-editor/src/components/ui/calendar.tsx
  code-editor/src/components/ui/card.tsx
  code-editor/src/components/ui/carousel.tsx
  code-editor/src/components/ui/chart.tsx
  code-editor/src/components/ui/checkbox.tsx
  code-editor/src/components/ui/collapsible.tsx
  code-editor/src/components/ui/command.tsx
  code-editor/src/components/ui/context-menu.tsx
  code-editor/src/components/ui/dialog.tsx
  code-editor/src/components/ui/drawer.tsx
  code-editor/src/components/ui/dropdown-menu.tsx
  code-editor/src/components/ui/empty.tsx
  code-editor/src/components/ui/field.tsx
  code-editor/src/components/ui/form.tsx
  code-editor/src/components/ui/hover-card.tsx
  code-editor/src/components/ui/input-group.tsx
  code-editor/src/components/ui/input-otp.tsx
  code-editor/src/components/ui/input.tsx
  code-editor/src/components/ui/item.tsx
  code-editor/src/components/ui/kbd.tsx
  code-editor/src/components/ui/label.tsx
  code-editor/src/components/ui/menubar.tsx
  code-editor/src/components/ui/navigation-menu.tsx
  code-editor/src/components/ui/pagination.tsx
  code-editor/src/components/ui/popover.tsx
  code-editor/src/components/ui/progress.tsx
  code-editor/src/components/ui/radio-group.tsx
  code-editor/src/components/ui/resizable.tsx
  code-editor/src/components/ui/scroll-area.tsx
  code-editor/src/components/ui/select.tsx
  code-editor/src/components/ui/separator.tsx
  code-editor/src/components/ui/sheet.tsx
  code-editor/src/components/ui/sidebar.tsx
  code-editor/src/components/ui/skeleton.tsx
  code-editor/src/components/ui/slider.tsx
  code-editor/src/components/ui/sonner.tsx
  code-editor/src/components/ui/spinner.tsx
  code-editor/src/components/ui/switch.tsx
  code-editor/src/components/ui/table.tsx
  code-editor/src/components/ui/tabs.tsx
  code-editor/src/components/ui/textarea.tsx
  code-editor/src/components/ui/toast.tsx
  code-editor/src/components/ui/toaster.tsx
  code-editor/src/components/ui/toggle-group.tsx
  code-editor/src/components/ui/toggle.tsx
  code-editor/src/components/ui/tooltip.tsx
  code-editor/src/hooks/use-mobile.tsx
  code-editor/src/hooks/use-toast.ts
  code-editor/src/index.css
  code-editor/src/lib/ai-service.ts
  code-editor/src/lib/github-service.ts
  code-editor/src/lib/projects.ts
  code-editor/src/lib/store.ts
  code-editor/src/lib/tts-service.ts
  code-editor/src/lib/utils.ts
  code-editor/src/lib/virtual-fs.ts
  code-editor/src/lib/zip-service.ts
  code-editor/src/main.tsx
  code-editor/tsconfig.json
  code-editor/vite.config.ts
  mockup-sandbox/.replit-artifact/artifact.toml
  mockup-sandbox/components.json
  mockup-sandbox/index.html
  mockup-sandbox/mockupPreviewPlugin.ts
  mockup-sandbox/package.json
  mockup-sandbox/src/.generated/mockup-components.ts
  mockup-sandbox/src/App.tsx
  mockup-sandbox/src/components/ui/accordion.tsx
  mockup-sandbox/src/components/ui/alert-dialog.tsx
  mockup-sandbox/src/components/ui/alert.tsx
  mockup-sandbox/src/components/ui/aspect-ratio.tsx
  mockup-sandbox/src/components/ui/avatar.tsx
  mockup-sandbox/src/components/ui/badge.tsx
  mockup-sandbox/src/components/ui/breadcrumb.tsx
  mockup-sandbox/src/components/ui/button-group.tsx
  mockup-sandbox/src/components/ui/button.tsx
  mockup-sandbox/src/components/ui/calendar.tsx
  mockup-sandbox/src/components/ui/card.tsx
  mockup-sandbox/src/components/ui/carousel.tsx
  mockup-sandbox/src/components/ui/chart.tsx
  mockup-sandbox/src/components/ui/checkbox.tsx
  mockup-sandbox/src/components/ui/collapsible.tsx
  mockup-sandbox/src/components/ui/command.tsx
  mockup-sandbox/src/components/ui/context-menu.tsx
  mockup-sandbox/src/components/ui/dialog.tsx
  mockup-sandbox/src/components/ui/drawer.tsx
  mockup-sandbox/src/components/ui/dropdown-menu.tsx
  mockup-sandbox/src/components/ui/empty.tsx
  mockup-sandbox/src/components/ui/field.tsx
  mockup-sandbox/src/components/ui/form.tsx
  mockup-sandbox/src/components/ui/hover-card.tsx
  mockup-sandbox/src/components/ui/input-group.tsx
  mockup-sandbox/src/components/ui/input-otp.tsx
  mockup-sandbox/src/components/ui/input.tsx
  mockup-sandbox/src/components/ui/item.tsx
  mockup-sandbox/src/components/ui/kbd.tsx
  mockup-sandbox/src/components/ui/label.tsx
  mockup-sandbox/src/components/ui/menubar.tsx
  mockup-sandbox/src/components/ui/navigation-menu.tsx
  mockup-sandbox/src/components/ui/pagination.tsx
  mockup-sandbox/src/components/ui/popover.tsx
  mockup-sandbox/src/components/ui/progress.tsx
  mockup-sandbox/src/components/ui/radio-group.tsx
  mockup-sandbox/src/components/ui/resizable.tsx
  mockup-sandbox/src/components/ui/scroll-area.tsx
  mockup-sandbox/src/components/ui/select.tsx
  mockup-sandbox/src/components/ui/separator.tsx
  mockup-sandbox/src/components/ui/sheet.tsx
  mockup-sandbox/src/components/ui/sidebar.tsx
  mockup-sandbox/src/components/ui/skeleton.tsx
  mockup-sandbox/src/components/ui/slider.tsx
  mockup-sandbox/src/components/ui/sonner.tsx
  mockup-sandbox/src/components/ui/spinner.tsx
  mockup-sandbox/src/components/ui/switch.tsx
  mockup-sandbox/src/components/ui/table.tsx
  mockup-sandbox/src/components/ui/tabs.tsx
  mockup-sandbox/src/components/ui/textarea.tsx
  mockup-sandbox/src/components/ui/toast.tsx
  mockup-sandbox/src/components/ui/toaster.tsx
  mockup-sandbox/src/components/ui/toggle-group.tsx
  mockup-sandbox/src/components/ui/toggle.tsx
  mockup-sandbox/src/components/ui/tooltip.tsx
  mockup-sandbox/src/hooks/use-mobile.tsx
  mockup-sandbox/src/hooks/use-toast.ts
  mockup-sandbox/src/index.css
  mockup-sandbox/src/lib/utils.ts
  mockup-sandbox/src/main.tsx
  mockup-sandbox/tsconfig.json
  mockup-sandbox/vite.config.ts
```

---

*Plano gerado pelo SK Code Editor — 25/04/2026, 00:39:23*