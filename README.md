# Cold Tech Aracaju
Site de apresentação responsivo, HTML/CSS/JS sem dependências de build. Sirva `dist/` via HTTP. Não abrir index.html diretamente com file:// (content.json usa fetch).

Contato confirmado no Instagram em 19/11/2026: +55 79 99837-1420. Marca, imagens e serviços extraídos do perfil público https://www.instagram.com/coldtech.aju/. Endereço completo, horários e CNPJ não foram confirmados e não são inventados. O Maps abre uma busca, não um endereço validado. As imagens locais são cópias das publicações da própria empresa, sem URLs temporárias de CDN.

O site é uma apresentação, com noindex. Não tem CRM, banco, login, rastreadores nem coleta de dados. O formulário apenas monta uma mensagem para revisão no WhatsApp.

## Conteúdo
`dist/content.json` concentra contato e galeria; `dist/assets/` contém imagens locais. Textos institucionais estão no HTML. Ver `docs/CRM-INTEGRATION.md` para a preparação futura. Nenhuma integração foi ativada.

## Validação
`node --check dist/app.js`; validar JSON e links locais. Prévia via servidor estático.
