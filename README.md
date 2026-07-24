# Blessy Vida Leve — página de produto

Site estático. Nada para compilar.

## Estrutura
```
index.html      página completa
support.js      runtime necessário (não remover)
assets/         imagens, logo e vídeos
vercel.json     cache dos assets
```

## Publicar na Vercel com GitHub
1. Crie um repositório no GitHub e envie **todo o conteúdo desta pasta na raiz** (index.html no primeiro nível).
2. Na Vercel: **Add New → Project → Import** o repositório.
3. Framework Preset: **Other**. Build Command: vazio. Output Directory: vazio (raiz).
4. Deploy. Depois adicione seu domínio em Settings → Domains.

## Onde editar
Tudo fica no `index.html`:
- **CFG** (topo do script): preços, Pix, cronômetro, WhatsApp, dados da empresa, política de troca, URL do checkout.
- **FLAVORS**: sabores, descrições e imagens.
- **STORIES**: vídeos em destaque.
- **REVIEWS**: avaliações (hoje são demonstrativas — substituir por reais antes de anunciar).
- **infoRotulo**: ingredientes, informação nutricional, alérgicos e advertências por sabor (preencher com o texto impresso no rótulo).

## Meta Pixel
Pixel `1028592796448984` já instalado com PageView, ViewContent, AddToCart, InitiateCheckout, AddToWishlist, Contact e eventos customizados.
O evento **Purchase** deve ser disparado na página de obrigado do checkout.
O token da API de Conversões **não** foi incluído no código (não deve ficar exposto no site) — use-o apenas no servidor.
