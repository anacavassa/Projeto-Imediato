# Simulador grátis — Projeto Imediato

Consulta de imóvel em Campinas: endereço → código cartográfico, bairro, zona e foto aérea
oficial da Prefeitura. Ao final, monta o resumo e entrega no WhatsApp já preenchido.

**Testado e funcionando em 06/09/2026** (endereço de teste devolveu código, bairro, zona,
ortofoto e limites de lote).

## Os 3 arquivos

| Arquivo | Tamanho | O que é |
|---|---|---|
| `index.html` | 22 KB | o simulador inteiro (7 etapas, mapa, WhatsApp) |
| `dados.js` | 8,2 MB | 9.294 logradouros + 13.740 imóveis com código cartográfico |
| `README.md` | — | este arquivo |

O bloco `LOTES` foi retirado do `dados.js` em 06/09/2026 — o simulador não usa (os limites de
lote vêm do WMS da Prefeitura, ao vivo). Economia de 5 MB no carregamento.
A versão completa está guardada em `..\dados-completo-com-lotes.js`.

## Como colocar no ar (GitHub Pages) — 5 minutos

1. Abrir `https://github.com/anacavassa/Projeto-Imediato`
2. **O repositório precisa ser público.** GitHub Pages de graça só funciona em repositório
   público. Se estiver privado: *Settings* → rolar até *Danger Zone* → **Change visibility** →
   *Make public*
3. Na aba **Code**: botão **Add file** → **Upload files** → arrastar os **3 arquivos**
   desta pasta → **Commit changes**
4. **Settings** (do repositório) → menu lateral **Pages** → em *Build and deployment*,
   *Source* = **Deploy from a branch**, *Branch* = **main** e pasta **/ (root)** → **Save**
5. Esperar de 1 a 3 minutos. O endereço fica:
   **https://anacavassa.github.io/Projeto-Imediato/**

Depois disso o botão entra na página `/simulador/` do site.

## Vídeo

GitHub aceita vídeo (até 100 MB por arquivo). O `IMG_3767.MOV` precisa ser convertido para
`.mp4` antes — navegador não toca `.MOV` de iPhone de forma confiável. Uma vez convertido,
sobe junto e entra na página com `<video controls>`.

## Por que não fica dentro do WordPress

O plano Pessoal do WordPress.com apaga `<script>` **e** `<iframe>` (testado em 06/09/2026).
Não existe forma de embutir. As opções são: hospedar fora (isto aqui) ou subir para o plano
Negócios — R$ 2.088 por 3 anos.
