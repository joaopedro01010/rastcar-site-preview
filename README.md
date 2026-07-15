# site-rastcar-x — Rastcar (estilo SpaceX/Starlink)

Site institucional one-page, estático e self-contained, no estilo cinematográfico da SpaceX/Starlink: **preto absoluto + tipografia branca seca + Champagne Gold como único acento**. Construído do zero, separado do `../site-rastcar/` (que continua intacto).

## Como abrir
```
cd site-rastcar-x && python3 -m http.server 8731
# http://localhost:8731
```
Ou abra `index.html` direto (tudo é relativo; só precisa servir por causa das fontes/imagens).

## Estrutura — 7 cenas full-screen (scroll)
1. **Hero** — foto carro à noite · "Para quem não aceita perder o que construiu"
2. **Rastreamento** — mapa/HUD em SVG (ponto gold + cerca virtual) · "Onde ele estiver. Agora."
3. **Controle** — foto detalhe noturno · bloqueio remoto + cerca · "O controle na sua mão"
4. **Frota** — foto frota · telemetria + 40 relatórios · "Dados. O ativo mais valioso do mundo."
5. **Cobertura** — foto Terra/América do Sul · "Do Brasil à Argentina. Sem fronteiras"
6. **Prova** — números (20+ anos, 24h, 40+, BR·AR) + Zelo (calor humano, discreto)
7. **CTA** — R$89,90/mês · instalação R$197 · WhatsApp + (12) 3157-9090

## Assets (`assets/`)
- `hero.jpg`, `bloqueio.jpg`, `frota.jpg`, `cobertura.jpg` — fundos gerados no Higgsfield (nano_banana 2K, recomprimidos com sips; site inteiro ~1,8 MB).
- `emblem.png` — emblema R dourado (nav + favicon). `wordmark-white.png` — wordmark off-white. `zelo.png` — mascote (só na cena 06).

## Travas de marca respeitadas
- Cobertura **nacional + Argentina** — zero "Vale do Paraíba"/"região".
- **Sem** menção a sensor de combustível.
- Slogan **PF** no hero ("Para quem não aceita perder o que construiu") · slogan **PJ** na frota ("Dados. O ativo mais valioso do mundo.").
- Zelo usado com parcimônia (um único ponto de calor humano).

## Stack
HTML único + CSS embutido + JS mínimo (IntersectionObserver pra scroll-reveal, menu mobile, nav blur no scroll). Fontes: Sora (títulos) + Hanken Grotesk (corpo) via Google Fonts. `prefers-reduced-motion` respeitado.
