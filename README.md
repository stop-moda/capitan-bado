# Stop Moda Masculina, Capitán Bado: página do grupo VIP

Página estática (HTML + CSS + JS, sem build). É cópia do site de Ponta Porã (`sites\stop-moda`) com a cidade trocada para **Capitán Bado, Paraguai**.

Endereço no ar: https://stop-moda.github.io/capitan-bado/ (repositório `stop-moda/capitan-bado`, depois de publicado).

## Como rodar

```bash
python -m http.server 5175
```

Abra http://localhost:5175.

## Estrutura

- `index.html`, `style.css`, `script.js`
- `assets/`: logo (SVG), favicon, ícone do iPhone, imagem de compartilhamento
- `public/images/`: fotos otimizadas em WebP

## Como mexer

- **Link do grupo:** `CONFIG.GROUP_LINK` no topo do `script.js`. Vale para os 3 botões. Tem que ser o grupo de Capitán Bado, não o de Ponta Porã.
- **Fotos da faixa:** os `<li class="strip__item">` do único grupo em `.strip`, no `index.html`.
- **Texto das faixas de alerta:** atributo `data-words` das duas `.tape__track` no `index.html`, palavras separadas por `|`.
- **Cidade:** aparece no topo, no texto principal, nas faixas, no bloco vermelho, no rodapé, no título e nos dados estruturados. Para trocar, procurar por "Capitán Bado".
- Não mencionar a unidade de Ponta Porã nesta página.

## Pendências

- **Link do grupo VIP de Capitán Bado:** colar em `script.js`. Enquanto estiver vazio, os botões mostram um aviso. **Não divulgar antes disso.**
- **Endereço, telefone e Instagram da loja:** não informados.
- **Domínio próprio:** ainda não definido.
- **Idioma:** está em português. Confirmar com o cliente se prefere espanhol.
- **Textos:** o cliente precisa aprovar.
