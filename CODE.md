# Codigo feito em Python
```
import pandas as pd
df = pd.read_excel('base_notas.xlsx')
df['Média'] = df[['Nota1', 'Nota2', 'Nota3', 'Nota4']].mean(axis=1)
df.to_excel('nota_aluno.xlsx', index=False)
```

`import pandas as pd`: Isso traz para o código uma ferramenta chamada Pandas e a chama de "pd" para facilitar seu uso.

`df = pd.read_excel('base_notas.xlsx')`: Aqui, o código lê um arquivo Excel chamado 'base_notas.xlsx' e cria uma espécie de tabela chamada DataFrame (representada por "df") para armazenar esses dados.

`df['Média'] = df[['Nota1', 'Nota2', 'Nota3', 'Nota4']].mean(axis=1)`: Ele calcula a média das notas para cada aluno (cada linha) e cria uma nova coluna chamada 'Média' para armazenar essas médias.

`df.to_excel('nota_aluno.xlsx', index=False)`: Por fim, o código salva essa tabela modificada em um novo arquivo Excel chamado 'nota_aluno.xlsx'. A parte index=False significa que não queremos incluir na planilha o número que identifica cada linha.
