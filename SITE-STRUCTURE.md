# AntiBet Alerta: estrutura semântica do site

Última revisão: 2026-07-29

## Publicação

- Domínio canônico: `https://home.antibetalerta.com/`
- Página publicada: `index.html`
- Idioma: português do Brasil (`pt-BR`)
- Plataforma do aplicativo: Android 7.0 ou superior
- Instalação oficial: `https://play.google.com/store/apps/details?id=com.antibet.alerta`
- Guia indexável: `https://home.antibetalerta.com/como-bloquear-sites-de-apostas/`

## Hierarquia da página

| Ordem | ID | Finalidade |
| --- | --- | --- |
| 1 | `hero` | Identificar o produto, sua proposta principal e a ação de download. |
| 2 | `sobre` | Declarar fatos canônicos: finalidade, plataforma, Acessibilidade, privacidade, limites e autoria. |
| 3 | `problema` | Contextualizar o problema de apostas e apresentar estatísticas. |
| 4 | `como-funciona` | Explicar o fluxo entre detecção, intervenção, bloqueio, alerta e apoio. |
| 5 | `funcionalidades` | Apresentar os recursos disponíveis. |
| 6 | `bloqueio` | Delimitar o que o aplicativo bloqueia e o que não controla. |
| 7 | `protecao-em-camadas` | Recomendar uso complementar com outras ferramentas. |
| 8 | `privacidade` | Explicar quais dados são usados e onde permanecem. |
| 9 | `tecnologia` | Explicar as sete formas de detecção em linguagem acessível. |
| 10 | `apoio` | Direcionar para recursos externos de ajuda. |
| 11 | `faq` | Responder dúvidas comuns antes da instalação. |
| 12 | `download` | Repetir disponibilidade e ação principal. |

## Fontes de verdade

| Assunto | Fonte canônica |
| --- | --- |
| Conteúdo público e afirmações sobre o produto | `index.html` |
| Resumo para sistemas compatíveis | `llms.txt` |
| Identidade estruturada | JSON-LD no `<head>` de `index.html` |
| Rastreamento | `robots.txt` e `sitemap.xml` |
| Privacidade detalhada | `https://privacidade.antibetalerta.com/` |
| Distribuição do aplicativo | Google Play Store |
| Orientação sobre proteção em camadas | `como-bloquear-sites-de-apostas/index.html` |

## Entidades declaradas no JSON-LD

- `WebSite`: o domínio oficial.
- `WebPage`: a página inicial e sua data de revisão.
- `Organization`: o projeto AntiBet Alerta.
- `Person`: Brenda Bispo, criadora e desenvolvedora.
- `MobileApplication` e `SoftwareApplication`: o aplicativo Android, seus requisitos, preço e recursos.
- `Article`, `FAQPage` e `BreadcrumbList`: o guia sobre bloqueio em camadas, suas perguntas frequentes e navegação.

## Regras de consistência

1. O conteúdo visível, o JSON-LD e o `llms.txt` devem declarar os mesmos fatos.
2. O uso do Serviço de Acessibilidade deve permanecer explícito.
3. O aplicativo não deve ser descrito como tratamento médico nem como bloqueio infalível.
4. A privacidade deve ser explicada sem sugerir coleta remota de dados de uso.
5. Materiais em `play-store/`, `social-media/` e na implementação antiga `antibet-your-shield/` não definem o conteúdo publicado.
