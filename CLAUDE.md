# Notas do ambiente

As skills do HyperFrames (vídeo com HTML) ficam em `.claude/skills/`
(hyperframes, hyperframes-cli, hyperframes-registry, media-use).

Na sessão na nuvem, antes de renderizar:

- `npx hyperframes browser ensure` (baixa o Chrome headless usado no render).
- `cdn.jsdelivr.net` é bloqueado pela rede. Baixe as bibliotecas pelo npm e
  use cópia local, por exemplo GSAP:
  `npm pack gsap@3.14.2 && tar xzf gsap-3.14.2.tgz && mkdir -p vendor && cp package/dist/gsap.min.js vendor/`
  e troque o `<script src>` do CDN por `vendor/gsap.min.js`.
