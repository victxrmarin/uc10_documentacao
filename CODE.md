# Codigo feito em Python
```
import pandas as pd
df = pd.read_excel('base_notas.xlsx')
df['Média'] = df[['Nota1', 'Nota2', 'Nota3', 'Nota4']].mean(axis=1)
df.to_excel('nota_aluno.xlsx', index=False)
```
