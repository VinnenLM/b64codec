# b64codec

Ferramenta web para **codificar e decodificar Base64**, de texto e de imagens. Roda inteiramente no navegador: nada é enviado para servidor.

**Demo:** https://vinnenlm.github.io/b64codec/

## O que faz

- **Texto → Base64**: suporta acentos e emojis (UTF-8), com opção de Base64 *URL-safe* e de incluir ou remover o padding (`=`).
- **Base64 → Texto**: aceita Base64 padrão e URL-safe, com ou sem padding.
- **Imagem → Base64**: arraste ou escolha uma imagem, veja a pré-visualização e copie o resultado, com ou sem o prefixo `data:image/...;base64,`.
- **Base64 → Imagem**: cole o Base64 (com ou sem prefixo `data:`), o formato é detectado automaticamente (PNG, JPG, GIF, WebP, BMP, ICO, SVG), e você pode baixar a imagem.
- Botões de copiar e limpar, tema claro/escuro automático e layout responsivo, com menu lateral.

## Privacidade

Todo o processamento acontece localmente, com as APIs do navegador (`btoa`, `atob`, `TextEncoder`, `FileReader`, `Blob`). Não há back-end, requisições externas nem armazenamento de dados.

> Base64 é apenas uma codificação, **não é criptografia**. Não use para proteger informações sensíveis.

## Como usar localmente

É um único arquivo, sem dependências nem build:

```bash
git clone https://github.com/VinnenLM/b64codec.git
cd b64codec
# abra o index.html no navegador
```

## Publicação

Como é um site estático, pode ser hospedado em qualquer serviço do tipo (GitHub Pages, Netlify, Cloudflare Pages etc.), sem back-end. Este projeto usa o **GitHub Pages**, a partir da branch `main`.

## Tecnologias

HTML, CSS e JavaScript puros.
