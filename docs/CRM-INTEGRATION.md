# Integração futura — desativada

Não há integração ativa, credenciais, chamadas Supabase/Union ou endpoint de upload.

## Contrato existente
`dist/content.json`, schemaVersion 1, contém company e gallery. A página consome esse arquivo em leitura; falhas preservam o contato básico. Os dados da galeria são inseridos como textContent, sem HTML arbitrário.

## Etapa após aprovação
1. Confirmar logo em alta resolução, endereço, horários, serviços e autorização de uso das imagens.
2. Transferir os textos institucionais do HTML para o modelo de conteúdo completo do CRM.
3. Criar registros por empresa/site e permissão específica de edição/publicação. Não usar credenciais de serviço no navegador.
4. Upload no CRM: validar tamanho, MIME e assinatura do arquivo; remover metadados e gerar formatos/tamanhos otimizados. Armazenar em prefixo por empresa com autorização no servidor.
5. Publicação explícita: rascunho, prévia, revisão e versão publicada; gerar snapshot JSON público sanitizado, compatível com o contrato atual, com cache e invalidação ao publicar. Não consultar o CRM a cada visitante.
6. Endereços de mídia estáveis e CDN; histórico e rollback. Evitar URLs assinadas que expiram no conteúdo público.
7. Validar isolamento entre empresas, segurança dos uploads e reversão antes de ativar.

Nenhum esquema SQL, migração ou configuração no CRM existente foi aplicado.
