**Aula de introdução ao R**
# PRIMEIRA AULA - 02/03/2026

1. Leve introdução ao R, contando uma história da linguagem de programação;
2. O R é uma linguagem herdada da linguagem S;
3. Possui uma extensa documentação mas é limitado devido ao uso da memória RAM;
4. os dois principais repositórios utiizados no R são: Cran e Bioconductor;
5. Todos os valores no R são vetores, então é possível ter vetores de diferentes complexidade;
6. Vetores numéricos podem ser diviidios em tres grupos, os numeric (vetor de números reais), integer (vetores de números inteiros) e complex( vetores de números complexos);
7. Parindo para o Rstudio. é sempre bom ver onde o script que  será utilizado esta localizado, dentro do script é possível utilizar atralhos (Ctrl + enter) para rodar uma linha do script;


# SEGUNDA AULA - 03/03/2026

1. Fução append, serve para adicionar números entres os vetores que eu desejo posicionar. *EX* appende(X,y, after =3);
2. A função paste cola vetores;
3. A função grep retorna valores que eu estou procurando, utilizando fatores de bucas descritos pelo usuário.
   - grep (o que busca nos vetores, Variável que é utilizada), a função pode ser modificada mais ainda colocando "$" no final do que eu busco pra utilizar como se fosse um limitador até onde eu quero buscar. A função grep também pode ser alterada com ignore.case= T, a qual busca pelos caracteres em maiusculo.
4. para criar Lista basta usar o comando list;
   -Para acessar números dentro dentro uma lista, é necessário que seja entre chaves duplas;
   -A forma mais intuitiva de buscar um vetor da minha lista é: lista[[2]] [[2]]. O primeiro par de colchetes inidca a lista que eu irei buscar e o segundo ira indicar o vetor que eu vou buscar dentro da lista;
   - Uma lista pode ser uma dataflame, podendo trabalhar com uma vetor multi dimensional.
5. Para criar um dataflame, se utilizar a função dataflame e entre parênteses os valores que serão posto nesse dataflame;
   - É possível buscar ou extrair informações de dentro  do dataflame utlizando o seguinte comando: nome do dataflame+$ ---> o sifrão irá mostrar o que se podeteirar de dentro do dataflame.
   - Também é possível acessar uma dataflame do mesmo modo que uma matrix;
   - A organização da criação do dataflame é primero coluno e depois linha;
   - Pode ser buscado se uma informação de um dataflame está em outro.
      - *EX* dataflame1$nome_da_coluna_que_se_repetei%in%dataflame2$nome_da_coluna_que_se_repete
    
   - É possível unir dois dataflames eliminando informações que se repetem, deixando somente o que é único em cada um.
     - *EX* marge(dataflame1, dataflame2, by= nome_da_coluna_que_se_repete)
     - Caso alguns os datasflames tenha mais informações que o outro, é necessário indetinficar (all.dataflame=T)
