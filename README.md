# Clara — consulta de ações

Site estático para pesquisar ações brasileiras e consultar cotações históricas pela API pública da [brapi](https://brapi.dev/). A lista de ações fixadas fica salva no armazenamento local do navegador.

Os cenários indicativos analisam manchetes recentes do Google Notícias, acessadas por meio do proxy público CORS [cors.lol](https://cors.lol/), e combinam uma classificação simples de sentimento com a volatilidade histórica dos últimos três meses. Essa leitura automática pode errar ou não encontrar notícias. Os cenários não são recomendações, garantias nem preços-alvo. Cotações e notícias dependem de serviços externos e de conexão à internet.

## Recursos

- Fixe ações para acompanhar suas cotações. A lista é armazenada localmente no navegador.
- Consulte o histórico em gráficos de 1 dia, 5 dias, 1 mês, 6 meses, 1 ano ou 5 anos. O gráfico carrega os dados mais recentes ao abrir e atualiza a cada 30 minutos enquanto a página está visível; também pode ser atualizado manualmente.
- Simule uma aplicação fictícia com valor e datas escolhidos. O cálculo usa preços históricos e ações fracionárias, sem incluir taxas, impostos ou dividendos. O formulário e os resultados não são enviados a um servidor.
- Alterne entre o tema claro e o escuro; a preferência é salva no navegador.

Não há banco de dados, servidor próprio, backend ou chave de API privada no site. A disponibilidade de cotações e notícias depende dos serviços públicos externos.

## Publicar no GitHub Pages

1. Envie os arquivos deste projeto para a branch `main` do repositório.
2. No GitHub, abra **Settings → Pages**.
3. Em **Build and deployment**, selecione **Deploy from a branch**, escolha `main` e a pasta `/(root)`, e salve.
4. Abra a URL que o GitHub Pages disponibilizar.

As cotações precisam de conexão à internet. Elas podem apresentar atraso e são apenas para consulta, não constituindo recomendação de investimento.
