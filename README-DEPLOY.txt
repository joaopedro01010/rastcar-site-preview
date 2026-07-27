RASTCAR — SITE (deploy)
=======================
Site 100% estático (HTML/CSS/JS + assets). Não precisa de banco, build nem servidor de aplicação.

COMO SUBIR (Rigel):
1. Coloque TODO o conteúdo desta pasta na raiz pública do domínio (ex.: public_html / www).
2. A página inicial é index.html.
3. Páginas: index.html, equipamentos.html, produto.html (usa ?p=slug).
4. Mantenha a pasta assets/ (fontes, imagens, vídeos) junto — caminhos são relativos.
5. Recomendado: HTTPS. Nenhuma variável de ambiente é necessária.

Idiomas: PT/ES/EN/HE (troca pelo seletor; também aceita ?lang=en etc).
