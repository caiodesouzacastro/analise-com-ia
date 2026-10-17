# Prompts por etapa da análise

Troque o que está entre colchetes. Ao fim de cada etapa há um ponto de conferência humana: a etapa seguinte só começa depois dele. Nenhum texto entra numa ferramenta antes de anonimizado.

## Dados qualitativos

### 1 · Preparar e anonimizar

Faça a anonimização antes, à mão ou na ferramenta institucional. O prompt abaixo é uma segunda conferência e a divisão em trechos.

```
O texto abaixo é uma transcrição já anonimizada. Não resuma e não reescreva nada. Faça duas coisas:
1. Liste qualquer nome próprio, nome de escola, de cidade ou outro detalhe que ainda possa identificar a pessoa, com a frase em que aparece.
2. Divida a transcrição em trechos curtos, um por assunto, com identificador [P1]-01, [P1]-02 e assim por diante, mantendo o texto exatamente como está.
Transcrição: [cole a transcrição anonimizada]
```

Conferência humana: buscar nomes próprios no arquivo antes de seguir.

### 2 · Definir a pergunta e o livro de códigos

```
Vou analisar entrevistas para responder à pergunta abaixo. Proponha um rascunho de livro de códigos curto, com no máximo oito códigos. Para cada código: uma sigla de três letras, um nome e uma definição de uma linha. Inclua a regra para quando nenhum código couber (SEM CÓDIGO). Aponte os pares de códigos que podem dizer quase a mesma coisa. Não codifique nada ainda.
Pergunta da análise: [cole a pergunta]
Contexto das entrevistas: [quem foi entrevistado e sobre o quê]
```

Conferência humana: a equipe fecha o livro; quem conhece o tema revisa se os códigos cobrem o que importa.

### 3 · Testar o livro de códigos com a IA

```
Aplique o livro de códigos abaixo aos trechos de amostra. Para cada trecho, indique o código, ou SEM CÓDIGO, e a citação literal que o justifica. Depois, liste todas as dúvidas que você teve sobre o próprio livro: definições que não deixam claro se um trecho entra, códigos que se sobrepõem e situações que nenhum código cobre. Não corrija o livro; só aponte as dúvidas.
Livro de códigos: [cole o livro]
Trechos de amostra: [cole de 5 a 10 trechos]
```

Conferência humana: ajustar o livro antes de codificar o conjunto todo.

### 4 · Codificar com livro fechado

Este é o Prompt 1 do exercício. Troque "a formação" pelo tema da sua análise e cole o livro de códigos e os trechos no lugar dos colchetes.

```
Você vai codificar trechos de entrevistas usando apenas o livro de códigos abaixo. Regras: use só os códigos do livro; um trecho pode ter mais de um código ou nenhum, e quando nenhum couber marque SEM CÓDIGO; para cada código aplicado, copie entre aspas a frase exata do trecho que o justifica; indique se a fala é positiva, negativa, neutra ou mista sobre a formação, e marque DÚVIDA quando não der para saber; não resuma e não interprete além do texto. Devolva uma tabela com: ID do trecho, código, citação literal, tom e observação.
[livro de códigos]
[trechos]
```

Conferência humana: nenhum código vale sem citação; a etapa 5 vem antes de qualquer resumo.

### 5 · Conferir citações e códigos

Rode num chat novo, sem o histórico da codificação.

```
Abaixo estão os trechos originais e uma codificação feita antes. Para cada linha da codificação, confira se a citação está no trecho letra por letra e se o código tem relação com a citação. Classifique cada linha como: confere; citação diferente do trecho; código sem relação com a citação; depende da fala anterior. Liste à parte os trechos com ironia ou fala ambígua. Não refaça a codificação.
Trechos: [cole os trechos]
Codificação: [cole a tabela]
```

Conferência humana: numa amostra de pelo menos 20%, comparar com a codificação de uma pessoa da equipe.

### 6 · Codificação aberta ou resumo

Este é o Prompt 2 do exercício. Troque "os professores" e "a formação continuada" pelo grupo e pelo tema da sua análise.

```
Leia os trechos abaixo e proponha categorias que descrevam o que os professores dizem sobre a formação continuada. Para cada categoria: nome, definição em uma linha, IDs dos trechos e uma citação literal de cada trecho. Liste à parte os trechos que não se encaixam em nenhuma categoria e as falas que destoam da maioria. Não junte falas de professores diferentes numa mesma citação.
[trechos]
```

Conferência humana: as categorias são pistas de temas novos, não conclusões; desconfie de categoria genérica que absorve qualquer fala.

### 7 · Procurar quem destoa, separado

```
Para cada entrevistado abaixo, separadamente, diga o que ele diz que nenhum dos outros diz: experiências, condições ou opiniões que só aparecem nas falas dele. Use citação literal com o ID do trecho. Não faça um resumo geral e não junte entrevistados.
Trechos, agrupados por entrevistado: [cole os trechos]
```

Conferência humana: quem conhece o tema confere se as vozes que destoam chegaram à síntese.

### 8 · Escrever a síntese

```
Com base apenas na codificação conferida abaixo, escreva uma síntese de até uma página que responda à pergunta: [cole a pergunta]. Cada afirmação termina com os IDs dos trechos que a sustentam, entre parênteses. Se disser quantos entrevistados mencionaram algo, use isso só como descrição, nunca como medida de importância. Inclua um parágrafo sobre quem destoa. Marque como [inferência] o que não estiver na codificação.
Codificação: [cole a tabela conferida]
```

Conferência humana: cada afirmação aponta para trechos, e a síntese não diz mais do que os trechos permitem.

### 9 · Registrar as decisões

```
Organize um registro curto desta análise com: pergunta, livro de códigos final, mudanças feitas no livro depois do teste e da conferência, prompts usados, ferramenta e data, número de trechos e decisões tomadas pela equipe. Use só as informações abaixo; o que faltar, marque [preencher].
Informações: [cole]
```

Conferência humana: o registro fica guardado junto da planilha de codificação.

## Dados quantitativos

### 1 · Dizer a unidade de contagem

```
Quero calcular o indicador abaixo. Antes de escrever qualquer código, diga qual unidade de contagem ele exige (pessoas, vínculos, matrículas, escolas ou outra) e que tipo de arquivo ou variável permite contar essa unidade sem contar o mesmo caso duas vezes. Não escreva código ainda.
Indicador: [descreva o que quer contar, o recorte e o ano]
```

Conferência humana: a equipe escreve a unidade de contagem antes de seguir.

### 2 · Mostrar à IA a estrutura real da base

```
Use só os nomes de arquivo e de coluna que aparecem abaixo; não invente nenhum. Se a base não tiver o que é preciso para contar a unidade [unidade], diga isso antes de escrever código. Depois, escreva o código e diga, linha por linha, que coluna usou e por quê.
Arquivo: [nome do arquivo e o que é cada linha]
Colunas: [cole a lista de colunas]
Dicionário: [cole o trecho do dicionário de dados das colunas que importam]
Indicador: [o que quer contar]
```

Conferência humana: cada nome de coluna do código existe na lista e no dicionário.

### 3 · Ler o código linha por linha

```
Explique o código abaixo linha por linha, em linguagem simples. Para cada linha, diga que filtro aplica, que variável usa e como trata valores vazios. No fim, diga o que exatamente o resultado mede e se o rótulo que o código imprime descreve isso. Se não descrever, proponha um rótulo correto.
Código: [cole o código]
Unidade de contagem pretendida: [pessoas, vínculos, matrículas...]
```

Conferência humana: ler o print final do código e corrigir o rótulo.

### 4 · Reproduzir um número publicado

```
Adapte o código abaixo para calcular o mesmo indicador num recorte que já tem total publicado: [recorte, ano e publicação oficial]. Não mude a lógica, só o recorte. Quando eu colar o resultado e o número publicado, liste as explicações possíveis para a diferença, da mais provável para a menos provável, e diga em qual trecho do dicionário de dados cada uma se apoia. Não afirme nenhuma sem esse apoio.
Código: [cole o código]
```

Conferência humana: rode você mesmo e compare; o número só é usado depois que a diferença está explicada.

### 5 · Registrar

```
Organize um registro curto deste cálculo com: fonte, ano, arquivo, colunas usadas, código, resultado, número publicado de referência, diferença e a explicação da diferença. Use só as informações abaixo; o que faltar, marque [preencher].
Informações: [cole]
```

Conferência humana: o registro fica guardado junto do código.
