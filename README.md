# Family Garage

Painel mobile-first da família para registrar abastecimentos e trajetos de carros e moto. O site é publicado pelo GitHub Pages a partir da branch `main`.

## Dados compartilhados

O app usa o projeto Supabase dedicado `family-garage`, nas tabelas `family_entries` e `family_settings`. O link não exige login: qualquer pessoa que tiver o endereço pode consultar, adicionar e editar registros. O papel anônimo tem apenas permissões de leitura, inclusão e edição; o app não oferece exclusão.

Os registros que já estavam salvos no navegador são enviados uma vez ao banco na primeira conexão. O navegador mantém uma cópia local e uma fila para mudanças feitas sem internet, que são sincronizadas quando a conexão volta. O app atualiza o histórico compartilhado a cada 15 segundos.

## Veículos e consumo

- Ford Ka: 11 km/L
- Citroen C3: 11 km/L
- Triumph Speed 400 (mostrada como “Triumph”): consumo configurável; fica em branco até a média ser informada

O preço por litro e as médias de consumo são configurações compartilhadas e podem ser editados no painel.
