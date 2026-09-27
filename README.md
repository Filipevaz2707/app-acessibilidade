# app-acessibilidade

Aplicação web desenvolvida com foco em acessibilidade e performance.

![GitHub license](https://img.shields.io/github/license/Filipevaz2707/app-acessibilidade)
![GitHub last commit](https://img.shields.io/github/last-commit/Filipevaz2707/app-acessibilidade)

## 📖 Sobre o projeto

Este projeto tem como objetivo demonstrar boas práticas de desenvolvimento front-end, com especial atenção a:
- Acessibilidade (WCAG 2.1)
- Performance e otimização de recursos
- Estrutura semântica de HTML
- Boas práticas de versionamento e organização de repositório

## 🛠️ Tecnologias utilizadas

- HTML5 semântico
- CSS3 (variáveis customizadas para dark mode/alto contraste)
- JavaScript
- Vite (bundler e build de produção)
- WAI-ARIA (para componentes interativos)

## ✅ Pré-requisitos

Antes de começar, é necessário ter instalado:
- [Node.js](https://nodejs.org/) (versão 18 ou superior)
- [Git](https://git-scm.com/)

## 🚀 Instalação e execução local

```bash
# Clonar o repositório
git clone https://github.com/Filipevaz2707/app-acessibilidade.git

# Entrar na pasta do projeto
cd app-acessibilidade

# Instalar dependências
npm install

# Executar em ambiente de desenvolvimento
npm run dev

# Gerar build de produção
npm run build

# Testar a build de produção localmente
npm run preview
```

## 🌳 Estratégia de versionamento (GitFlow)

O projeto segue o modelo **GitFlow**, mesmo em desenvolvimento individual, para simular um fluxo colaborativo real:

- **`main`**: código estável, apenas versões lançadas (releases).
- **`develop`**: integração contínua do desenvolvimento.
- **`feature/`**: criadas a partir de `develop` para cada nova funcionalidade.
- **`hotfix/`**: partem de `main` para correções urgentes, depois mescladas em `main` e `develop`.

### Convenção de commits

Utiliza-se o padrão **Conventional Commits**:
- `feat:` nova funcionalidade
- `fix:` correção de bug
- `docs:` alterações na documentação
- `refactor:` refatoração sem alteração de comportamento
- `style:` formatação, sem alteração de lógica

### Versionamento semântico (SemVer)

Tags de release seguem o formato `MAJOR.MINOR.PATCH`:
- **MAJOR**: alterações incompatíveis
- **MINOR**: novas funcionalidades compatíveis
- **PATCH**: correções de bugs

## ♿ Acessibilidade

- Landmarks semânticos: `<header>`, `<nav>`, `<main>`, `<footer>`
- Atributos WAI-ARIA em modais, botões de ícone e formulários
- Navegação completa por teclado, com foco visível (`:focus-visible`)
- Contraste mínimo de 4.5:1 (WCAG AA), validado com WebAIM Contrast Checker
- Suporte a modo escuro e alto contraste via variáveis CSS

## ⚡ Performance

- Imagens otimizadas em formato WebP com fallback PNG/JPEG
- `srcset` e `sizes` para imagens responsivas
- `loading="lazy"` para imagens fora do viewport
- Minificação de JS/CSS via Vite (esbuild)

## 📦 Deploy

O deploy é feito automaticamente via **Vercel**, ligado à branch `main`. Cada push em `main` gera uma nova versão em produção; branches `develop`/`feature/` geram *preview deployments* automáticos.

🔗 **Aplicação em produção:** _(adicionar link do deploy aqui)_

## 📄 Licença

Este projeto está licenciado sob a licença MIT — veja o ficheiro [LICENÇA](./LICENÇA) para mais detalhes.

## 👤 Autor

**Filipe Vaz**
- GitHub: [@Filipevaz2707](https://github.com/Filipevaz2707)
