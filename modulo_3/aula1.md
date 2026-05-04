### Aula 1

## Visualizando e editando textos através da linha de comando
- wc -l <arquivo>               = quantas linhas no arquivo
- wc -c <arquivo>               = quantos caracteres no arquivo
- wc -w <arquivo>               = quantas palavras no arquivo
- cat  <arquivo>                = traz o conteúdo do arquivo, aceita multiplos arquivos, mas em sequência.
- more  <arquivo>               = traz o conteúdo em modo de "paginação"
- less <arquivo>                = usa a setas de movimentação do cursor, use numeros para ir pra linhas específicas
- cat > <arquivo>               = consegue criar o arquivo e escrever já em sequência, se existir, sobreencreve o arquivo
- cat >> <arquivo>              = append no arquivo existente
- tail -n 50 <arquivo>          = traz as últimas 10 informações, mas passando -n as útlimas <n> informações
- tail -f <arquivo>             = traz as atualizações em tempo real no arquivo, dinâmico
- diff  <arquivo1> <arquivo2>   = diferença entre os arquivos "Arquivo 1" é o original "Arquivo 2" é o testado. se vier < é que falta no testado(ou está a mais no original), se vier > falta no original(ou está a mais no testado) 
- diff -u <arquivo1> <arquivo2> = diferença mostrando as linhas --- +++, mostrando sempre em relação ao arquivo1 se precisa tirar ou colocar. (O que ta de diferente)


##  Tudo sobre o VIM
- yy = copia linha toda
- p = colar (paste)
- yw = palavra que esta no curso é copiada
- y<n>y = copia n linhas
- y<n>w = copia n palavras 
- d<n>d = deleta n linhas
- d<n>w = deleta n palavras
- o = inserção na linha de baixo
- O = inserção na linha de cima
- I = inserção no início da linha
- i = inserção no local do cursor
- a = inserção 1 caracter na frente
- A = inserção no final da linha
- v = visual, com as setas você seleciona o texto
- V = visual line, copia linha em linha
- :split <arquivo> = divide a tela na horizontal com o outro arquivo
- :vsplit <arquivo> = divide a tela na vertical com o outro arquivo
- :e <arquivo> = muda pro arquivo que deseja
- :r <arquivo> = coloca o conteudo do arquivo desejado, no arquivo atual
