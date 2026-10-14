# 📋 Plano do projeto: Caca-Bug (6)

_Gerado em 14/10/2026, 09:13:58 — sem IA, lendo os arquivos._

## 📊 Visão geral
| Item | Valor |
|---|---|
| Arquivos | 57 |
| Linhas | 3.546 |
| Telas/páginas | 1 |
| Rotas do backend | 0 |
| Chamadas do app | 3 |
| Tabelas do banco | 0 |
| Variáveis de ambiente | 3 |

**Linguagens:** JavaScript (25), Imagem (15), Outros (3), JSON (3), Markdown (3), YAML (2), Imagem SVG (2), CSS (1), Ícone (1), Python (1), HTML (1)

## 💡 O que fazer (em ordem)
1. 🧹 Tirar a Replit de 10 arquivo(s) (🏗️ Preparar → Fazer tudo)
2. 🔐 Criar um .env.example com: BASE_PATH, GITHUB_STEP_SUMMARY, PORT (os valores você coloca no servidor, nunca no código)
3. 📝 Criar um README.md explicando como rodar

## 🚀 Por onde começa
- `index.html`

## ⌨️ Comandos (package.json)
| Pasta | Comando | O que roda |
|---|---|---|
| . | `npm run desktop` | `electron .` |
| . | `npm run exe` | `electron-builder --win portable --publish never` |

## 📱 Telas e páginas
| Endereço | Arquivo |
|---|---|
| `index.html` | index.html |

## 🖥️ Rotas do backend
_Nenhum encontrado._

## 📡 O que o app pede ao servidor
| Método | Endereço | Onde |
|---|---|---|
| POST | `/models/${encodeURIComponent(c.modelo)}:generateContent` | ferramentas/cirurgiao.js |
| POST | `/messages` | ferramentas/cirurgiao.js |
| POST | `/chat/completions` | ferramentas/cirurgiao.js |

## 🔌 O que falta no backend
✅ Tudo que o app chama tem rota no projeto (ou o app não usa servidor).

## 🗄️ Banco de dados
_Nenhuma tabela encontrada._

## 🔐 Variáveis de ambiente (configurar no servidor)
- `BASE_PATH`
- `GITHUB_STEP_SUMMARY`
- `PORT`

_Só os nomes. Os valores (chaves, senhas) nunca vão no código nem no GitHub._

## 🤖 IA usada
- api.openai.com
- api.groq.com
- openrouter.ai
- generativelanguage.googleapis.com
- api.anthropic.com

## 🌐 Serviços de fora que ele acessa
- api.anthropic.com
- api.deepseek.com
- api.groq.com
- api.mistral.ai
- api.openai.com
- api.perplexity.ai
- api.x.ai
- cdn.jsdelivr.net
- cdnjs.cloudflare.com
- esm.sh
- expo.dev
- fonts.googleapis.com
- fonts.gstatic.com
- generativelanguage.googleapis.com
- github.com
- google.serper.dev
- nominatim.openstreetmap.org
- ns.adobe.com
- openapi.monica.im
- openrouter.ai
- pje.tjmg.jus.br
- pypi.org
- raw.github.com
- registry.npmjs.org
- stuartk.com
- stuk.github.io
- u.expo.dev
- unpkg.com
- www.google.com
- www.npmjs.com

## 🧹 Arquivos com coisa da Replit
- ferramentas/analisador-universal.js
- ferramentas/cirurgiao.js
- ferramentas/montar.py
- ferramentas/projeto-lab.js
- js/30-projeto.js
- js/60-comparar.js
- js/99-app.js
- js/lib/expo-core.js
- js/lib/plano-core.js
- service-worker.js

## 🔁 Roteiro para recriar fora da Replit
1. Importar o projeto no Mini SK e tocar em 🏗️ Preparar → ✅ Fazer tudo (tira a Replit, cria os arquivos que faltam).
2. Não tem backend: o site sozinho basta (Netlify ou GitHub Pages).
3. Variáveis: cadastrar 3 variável(is) no servidor (lista acima).
4. Testar a prévia; se der erro, 🤖 Mandar os erros para a IA.
5. App: 📲 Instalável (PWA), 📦 APK ou 🖥️ Desktop (.exe) pelo 🏗️ Preparar.

## 🌳 Árvore de arquivos
```
├─ 📁 .github/
│  └─ 📁 workflows/
│     ├─ apk.yml
│     └─ desktop-exe.yml
├─ 📁 css/
│  └─ app.css
├─ 📁 electron/
│  ├─ main.cjs
│  └─ preload.cjs
├─ 📁 ferramentas/
│  ├─ ai-code-studio.js
│  ├─ analisador-universal.js
│  ├─ cirurgiao.js
│  ├─ gerador-eas.js
│  ├─ limpador.js
│  ├─ montar.py
│  ├─ ordem.txt
│  ├─ perito.js
│  ├─ projeto-lab.js
│  └─ triagem.js
├─ 📁 icons/
│  ├─ apple-touch-icon.png
│  ├─ icon-128.png
│  ├─ icon-144.png
│  ├─ icon-152.png
│  ├─ icon-16.png
│  ├─ icon-180.png
│  ├─ icon-192.png
│  ├─ icon-32.png
│  ├─ icon-384.png
│  ├─ icon-48.png
│  ├─ icon-512.png
│  ├─ icon-72.png
│  ├─ icon-96.png
│  ├─ icon.svg
│  ├─ maskable-192.png
│  ├─ maskable-512.png
│  └─ maskable.svg
├─ 📁 js/
│  ├─ 📁 lib/
│  │  ├─ expo-core.js
│  │  ├─ organizar-core.js
│  │  └─ plano-core.js
│  ├─ 00-core.js
│  ├─ 20-zip.js
│  ├─ 30-projeto.js
│  ├─ 40-ferramentas.js
│  ├─ 45-organizar.js
│  ├─ 50-relatorios.js
│  ├─ 60-comparar.js
│  └─ 99-app.js
├─ 📁 lib/
│  ├─ diff-LICENSE.txt
│  ├─ diff.min.js
│  ├─ jszip-LICENSE.md
│  └─ jszip.min.js
├─ .gitignore
├─ apk.config.json
├─ favicon.ico
├─ index.html
├─ LEIA-ME.md
├─ manifest.json
├─ package.json
├─ PLANO.md
├─ service-worker.js
└─ sw.js
```
