# AntiBet Alerta: mapa do repositório

## Objetivo do domínio

Este repositório contém o site público do AntiBet Alerta, um aplicativo Android de apoio pessoal que identifica e bloqueia tentativas de acesso a sites de apostas. O site deve explicar o produto com linguagem simples, preservar a privacidade prometida e direcionar usuários para recursos de apoio.

## Entrada canônica

- `index.html`: página publicada em `https://home.antibetalerta.com/`; contém HTML, CSS e JavaScript da página estática.
- `llms.txt`: resumo factual e canônico do produto para leitores humanos e sistemas que adotem a convenção llms.txt.
- `robots.txt`: política de rastreamento e localização do sitemap.
- `sitemap.xml`: URLs indexáveis do domínio.
- `como-bloquear-sites-de-apostas/index.html`: guia editorial original sobre proteção em camadas, com fontes oficiais e dados estruturados de artigo.
- `favicon.svg`, `og-image.png`, `mockup.jpeg`: identidade e imagens públicas usadas pela página.

As pastas `play-store/` e `social-media/` contêm materiais de divulgação. A pasta `antibet-your-shield/` é uma implementação antiga e não é a origem do site publicado.

## Invariantes do produto

1. O app é gratuito, sem anúncios e sem cadastro obrigatório.
2. Os dados de uso permanecem no celular do usuário; não afirmar que são enviados para servidores do AntiBet Alerta.
3. O parceiro de apoio é opcional e recebe avisos por e-mail somente quando configurado pelo usuário.
4. O app usa o Serviço de Acessibilidade do Android, com consentimento, para ler somente o domínio na barra de endereço de navegadores compatíveis.
5. O produto é uma camada complementar; não prometer que bloqueia todos os sites nem apresentá-lo como tratamento médico.
6. A plataforma disponível é Android 7.0 ou superior. Não anunciar versão para iOS como disponível.
7. Não classificar o AntiBet Alerta como operador, afiliado ou promotor de apostas.

## Limites de edição

- Preserve o tom acolhedor, direto e não julgador.
- Mantenha afirmações do JSON-LD, `llms.txt` e conteúdo visível consistentes entre si.
- Não invente avaliações, número de instalações, certificações, acurácia ou garantias técnicas.
- Ao alterar URL, disponibilidade, versão ou política de dados, atualize todas as fontes canônicas na mesma mudança.
- Mantenha perguntas e respostas do JSON-LD idênticas ao FAQ visível do guia.
- Não edite materiais em `play-store/` ou `social-media/` quando a tarefa tratar apenas do site.

## Verificação mínima

```sh
xmllint --noout sitemap.xml
node -e "const fs=require('fs');const h=fs.readFileSync('index.html','utf8');const m=h.match(/<script type=\"application\\/ld\\+json\">([\\s\\S]*?)<\\/script>/);JSON.parse(m[1]);"
git diff --check
```
