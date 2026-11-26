# ExcelTitles

**Template + Legenda → Excel: alinhe o original em inglês e a tradução em uma planilha, legenda por legenda.**

O ExcelTitles junta a legenda template (inglês) e a legenda final (português) em um arquivo .xlsx com três colunas: tempo inicial, template e tradução. É útil para entregas que pedem planilha, revisões, relatórios e glossários.

## Formatos aceitos
SRT, DFXP, PXTT, TTML e TTAL (os dois arquivos podem estar em formatos diferentes).

## Funcionalidades
- **Pareamento automático** pela sobreposição de tempo, mesmo quando as legendas foram divididas ou mescladas de forma diferente nos dois arquivos. Cada legenda se liga só à do outro lado com a maior sobreposição, e as linhas seguem o tempo, então uma legenda longa não desalinha a cena inteira.
- **Linhas de continuação:** quando um lado tem mais divisões que o outro, as linhas extras ficam alinhadas, com o outro lado em branco.
- **Prévia na tela** antes de baixar:
  - amarelo: texto só de um lado;
  - verde: linha de continuação.
- **Timecode em frames** (HH:MM:SS:FF), com frame rate de 23,976 a 60. Se o template já estiver em timecode SMPTE, o frame rate é selecionado sozinho. Linhas que só existem na tradução também recebem o tempo inicial (o da tradução).
- **Explicações** (“?”) no frame rate, na tolerância e no deslocamento.
- **Tolerância de pareamento** (em segundos) para legendas sem sobreposição de tempo.
- **Deslocamento automático:** quando os arquivos começam em relógios diferentes (ex.: 01:00:00:00 em um e 00:00:00:00 no outro), o deslocamento é detectado e aplicado sozinho. Dá para alterar à mão, inclusive com valores negativos.
- **Resumo em etiquetas:** linhas geradas, legendas em cada arquivo, pareadas, continuações, sem par, deslocamento aplicado e aviso de poucos pares.
- **Itálico preservado** como `<i>` e quebras de linha mantidas dentro da célula.
- **Cabeçalho opcional** (Tempo Inicial / Template / Tradução), com a primeira linha congelada.
- Detecta UTF-8, UTF-16 e Windows-1252.
- Lê legendas SRT com linha em branco no meio do texto, timecode drop-frame em 29,97 e 59,94, e itálico de DFXP/TTML definido em estilos encadeados ou na região.
- O arquivo é salvo como `<nome do template>_alinhado.xlsx`.

## Privacidade
Tudo roda no seu navegador. Nada é enviado para lugar nenhum, e a planilha é gerada sem bibliotecas externas.
