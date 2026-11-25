# ExcelTitles

**Template + Legenda → Excel: alinhe o original em inglês e a tradução em uma planilha, legenda por legenda.**

O ExcelTitles junta a legenda template (inglês) e a legenda final (português) em um arquivo .xlsx com três colunas: tempo inicial, template e tradução. É útil para entregas que pedem planilha, revisões, relatórios e glossários.

## Formatos aceitos
SRT, DFXP, PXTT, TTML e TTAL (os dois arquivos podem estar em formatos diferentes).

## Funcionalidades
- **Pareamento automático** pela sobreposição de tempo, mesmo quando as legendas foram divididas ou mescladas de forma diferente nos dois arquivos.
- **Linhas de continuação:** quando um lado tem mais divisões que o outro, as linhas extras ficam alinhadas, com o outro lado em branco.
- **Prévia na tela** antes de baixar:
  - amarelo: texto só de um lado;
  - verde: linha de continuação.
- **Timecode em frames** (HH:MM:SS:FF), com frame rate de 23,976 a 60. Se o template já estiver em timecode SMPTE, o frame rate é selecionado sozinho.
- **Tolerância de pareamento** (em segundos) para legendas sem sobreposição de tempo.
- **Deslocar tradução:** corrige arquivos com timecodes iniciais diferentes (ex.: 01:00:00:00 em um e 00:00:00:00 no outro), aceitando valores negativos. Avisa quando encontra poucos pares.
- **Itálico preservado** como `<i>` e quebras de linha mantidas dentro da célula.
- **Cabeçalho opcional** (Tempo Inicial / Template / Tradução), com a primeira linha congelada.
- Detecta UTF-8, UTF-16 e Windows-1252.
- O arquivo é salvo como `<nome do template>_alinhado.xlsx`.

## Privacidade
Tudo roda no seu navegador. Nada é enviado para lugar nenhum, e a planilha é gerada sem bibliotecas externas.
