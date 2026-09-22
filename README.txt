LOFTS PRIME — CORREÇÃO FONTE ÚNICA

Arquivos:
- worker.js -> publicar no Cloudflare Worker lofts-prime-sync
- index.html -> publicar no Cloudflare Pages como página principal
- admin.html -> publicar no Cloudflare Pages como /admin
- legacy-canela/ -> fotos antigas de Canela usadas apenas uma vez para recuperação no painel

Mudanças principais:
1. Site público não usa mais anúncios/fotos embutidos no HTML como fallback.
2. Supabase/Worker passa a ser a fonte única de verdade.
3. Anúncio desativado não aparece no site.
4. Fotos públicas vêm somente do campo photos do loft no Supabase.
5. Reservas/availability usam dbId para também funcionar com anúncios importados.
6. Painel ganhou botão para recuperar as 10 fotos antigas de Canela.

Depois de publicar:
1. Entre no /admin.
2. Abra Fotos de Canela.
3. Clique em "Recuperar fotos antigas de Canela".
4. Confirme.
5. Confira que as fotos aparecem no painel.
6. Depois disso, as fotos antigas não são mais usadas pelo site público.

A pasta legacy-canela pode ser mantida por enquanto; ela não é usada para exibir anúncios no site.
