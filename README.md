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
- `assets/`: logo (SVG), favicon, ícone do iPhone, imagem de compartilhamento (só logo e texto, sem foto), `fonts/` (Barlow, hospedada no próprio site)

## Como mexer

- **Link do grupo:** `CONFIG.GROUP_LINK` no topo do `script.js`. Vale para os 3 botões.
- **Texto das faixas de alerta:** atributo `data-words` das duas `.tape__track` no `index.html`, palavras separadas por `|`.
- **Cidade:** aparece no topo, no texto principal, nas faixas, no bloco vermelho, no rodapé, no título e nos dados estruturados. Para trocar, procurar por "Capitán Bado".
- Não mencionar a unidade de Ponta Porã nesta página.

## Pendências

- **Link do grupo VIP:** já configurado em `CONFIG.GROUP_LINK` (`script.js`) com o grupo de WhatsApp informado em 2026-11-09, que é o **mesmo grupo dos dois sites**. Se a Stop criar um grupo só de Capitán Bado, é só trocar o link ali.
- **Texto "Grupo exclusivo para o público de Capitán Bado, no Paraguai.":** conflita um pouco com o fato de o grupo ser o mesmo nas duas cidades. Combinar com o cliente se mantém ou ajusta.
- **Endereço, telefone e Instagram da loja:** não informados.
- **Domínio próprio:** ainda não definido.
- **Idioma:** está em português. Confirmar com o cliente se prefere espanhol.
- **Textos:** o cliente precisa aprovar.
- **Fotos:** o cliente não gostou das fotos e todas foram retiradas (nos dois sites). Uma cópia fica fora do site, em `sites\_arquivo-fotos-removidas`. Elas continuam no histórico público do repositório no GitHub.
