<img src="Imagens do README/Cabecalho.png"/>

# Cubo Gelatinoso - Previsão de Desempenho Escolar com k-NN

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.13.7-blue">
  <img src="https://img.shields.io/badge/scikit--learn-KNN-green">
  <img src="https://img.shields.io/badge/Área-Machine%20Learning-darkred">
</p>

Notebook desenvolvido em Python pelo aluno Gustavo Junqueira Colas como projeto para a disciplina de Aprendizado de Máquina do segundo semestre da Ilum. O trabalho investiga o desempenho do algoritmo de *k*-vizinhos mais próximos (*k*-NN) na previsão da nota final de estudantes, a partir do **Student Performance Data Set** (Cortez & Silva, 2008). O trabalho testa exaustivamente diferentes combinações de hiperparâmetros (número de vizinhos, tipo de distância, ponderação dos vizinhos e conjunto de atributos utilizado), com e sem normalização dos dados, discutindo criticamente os resultados obtidos. Este projeto é a primeira entrega ("Cubo Gelatinoso") da disciplina Aprendizado de Máquina, ministrada pelo Prof. Dr. Daniel R. Cassar na Ilum Escola de Ciência, realizada individualmente pelo aluno Gustavo Junqueira Colas.

## Como executar:

1. Baixe ou clone o repositório e extraia os arquivos em uma pasta

2. Com o seu editor (preferencialmente o VSCode), vá em *File*, *Open Folder* e selecione a pasta baixada

3. Instale as dependências com o comando:
```sh
pip install -r requirements.txt
```

4. Abra o arquivo **Notebook_para_git.ipynb** e execute todas as células em ordem

## Conteúdo:

<ul>
  <li>:file_folder: <b>Imagens</b>: contém as imagens ilustrativas utilizadas ao longo do notebook</li>
    <ul>
      <li>:framed_picture: <b>L1.png</b>, <b>MAE.png</b>, <b>L2.png</b>, <b>RMSE.png</b>: ilustrações das métricas de perda discutidas na revisão teórica</li>
      <li>:framed_picture: <b>Dist_Minkowski.png</b>, <b>Dist_Chebyshev.png</b>: fórmulas das distâncias utilizadas pelo algoritmo</li>
      <li>:framed_picture: <b>Def_r2.png</b>: fórmula do coeficiente de determinação R²</li>
    </ul>
  <li>:notebook: <b>Notebook_Cubo.ipynb</b>: notebook completo, com revisão teórica, código comentado, resultados e conclusões</li>
  <li>:page_facing_up: <b>student-mat.csv</b>: dataset utilizado (Student Performance Data Set, Cortez &amp; Silva, 2008, UCI Machine Learning Repository)</li>
  <li>:spiral_notepad: <b>requirements.txt</b>: lista das bibliotecas necessárias para rodar o projeto</li>
</ul>

## Tecnologias Utilizadas:

O projeto foi confeccionado inteiramente em *Jupyter Notebook*, na linguagem *Python* (versão 3.13.7), utilizando as bibliotecas *pandas*, *scikit-learn*, *matplotlib*, *seaborn*, *scipy* e *numpy*, além dos módulos nativos *itertools*, *re* e *ast*. Inteligência artificial (na forma de *LLMs*) foi utilizada especialmente para formatação da linguagem *Markdown* (o que inclui o refinamento desse README) e para a disposição visualmente atraente dos gráficos utilizados no trabalho.

## Sobre o dataset e os atributos:

O modelo tem como objetivo prever a nota final do estudante (`G3`) a partir de atributos relacionados aos seus hábitos de estudo e ao seu contexto familiar:

| Atributo | Descrição |
|---|---|
| `studytime` | Tempo semanal dedicado ao estudo |
| `absences` | Número de faltas escolares |
| `freetime` | Tempo livre após a escola |
| `Mjob` / `Fjob` | Profissão da mãe / do pai (categóricas, codificadas para uso no modelo) |
| `Medu` / `Fedu` | Nível de escolaridade da mãe / do pai |
| `G1` | Nota do primeiro período (usada como nota anterior) |

## Hiperparâmetros investigados:

O notebook testa exaustivamente diferentes combinações de:
- Número de vizinhos (*k*)
- Tipo de distância (Manhattan, Euclidiana e uma terceira variante da família de Minkowski)
- Ponderação dos vizinhos (uniforme ou pelo inverso da distância)
- Conjunto de atributos utilizado
- Normalização dos dados (com e sem)

## Professor avaliador:

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/drcassar">
        <img src="https://avatars.githubusercontent.com/u/9871905?v=4" width="100px;" alt="Foto do Cassar no Github"/><br>
        <b>Prof. Dr. Daniel R. Cassar</b>
      </a>
    </td>
  </tr>
</table>

## Aluno:

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/gustavocolas-pessoal">
        <img src="https://avatars.githubusercontent.com/u/284495799?s=80&v=4" width="100px;" alt="Foto do Gustavo no Github"/><br>
        <b>Gustavo Junqueira Colas</b>
      </a>
    </td>
  </tr>
</table>
<img src="Imagens do README/Rodape.png"/>

