# Pandas: sum dataFrame rows for given columns

## 1. create a list of the columns and remove the ones you are not interested in
 col_list = list(df)
 col_list.remove('unwanting_col')
 df['sum'] = df[col_list].sum(axis=1)

### however this way is not convinent if there are several columns that you are not interested in

## 2. use location of column to sum dataFrame
 math_df['sum'] = math_df.iloc[:, 5:1032].sum(axis=1)

