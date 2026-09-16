# Rascunho — Segurança dos dados do Google Play

> Use como roteiro. As respostas finais devem refletir exatamente a versão enviada.

## Estado atual
- Não há conta própria do EQShift.
- Não há servidor próprio de usuários identificado no projeto atual.
- Não há captura/gravação do áudio reproduzido.
- O app acessa metadata de mídia: título, artista e álbum quando disponível.
- O app identifica tecnicamente o player ativo e a sessão necessária ao processamento.
- O app envia consultas de metadata musical a Deezer, Last.fm e MusicBrainz.
- Cache de análise: em memória, até ~50 resultados, TTL de até 6 horas.
- Preferências locais: onboarding, opções do app e modo desenvolvedor.
- Build release evita logs detalhados de metadata.

## Revisar antes de enviar
1. Confirmar se algum SDK adicional envia telemetria.
2. Confirmar ausência de analytics/crash reporting/publicidade.
3. Confirmar uso de HTTPS em todas as chamadas externas.
4. Manter a Política de Privacidade alinhada com o comportamento real.
