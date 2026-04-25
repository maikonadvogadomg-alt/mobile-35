# SK Code Editor

Editor de código mobile-first em português, com IA integrada, terminal, preview ao vivo, voz, automações de banco de dados, GitHub e ferramentas para criação rápida de apps.

Este projeto parece estar dividido em 3 partes principais:

- `code-editor/` → interface principal do editor
- `api-server/` → servidor de API que dá suporte às funções do editor
- `mockup-sandbox/` → ambiente separado para visualizar e testar mockups/componentes

---

## Visão geral

O SK Code Editor foi pensado para facilitar a criação, edição, teste e organização de projetos direto do navegador, com foco em produtividade e uso simples em dispositivos móveis.

### Principais recursos

- Editor de código com interface visual
- Assistente de IA integrado
- Terminal embutido
- Preview ao vivo
- Suporte a voz
- Integração com GitHub
- Backup e restauração
- Busca web
- Rotas de banco de dados
- Estrutura preparada para múltiplos módulos de frontend e backend

---

## Estrutura do projeto

```text
.
├── api-server/         # Backend/API do editor
├── code-editor/        # Aplicação principal do editor
├── mockup-sandbox/     # Sandbox para mockups e componentes
├── .sk/                # Arquivos internos de perfil/memória do assistente
├── SISTEMA.md          # Documento de informações do sistema
└── README.md           # Este arquivo