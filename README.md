# Projeto 1 da disciplina de Recuperação Inteligente de Informação

Utilização dos dados da página Americanas.com 

#### Primeira etapa:
Execução do crawler no notebook na pasta `crawler/Crawler dos dados dos produtos.ipynb`

Serão executadas as consultas celular e televisao na busca para a recuperação dos dados. O crawler busca o título e a 
descrição dos produtos retornados na busca.


#### Segunda etapa:

Cálculo da matriz de relevancia no notebook na pasta `relevancia/Criação da Matriz de relevancia.ipynb`
Escolhemos as consultas:

- televisão com tela de bordas infinitas
- smartphone samsung android com baterias de longa duração	

#### Terceira etapa:


Etapa de indexação e busca no Elasticsearch. Inicialmente executamos o Elasticsearch no docker-compose, com o seguinte comando no home desse projeto:

```
sudo docker-compose up 
```
Caso a execução não funcione, ocorreu um erro de memória na VM, então foi utilizado esse comando para corrigir o problema: `sudo sysctl -w vm.max_map_count=262144`.


Por fim, executamos o notebook na pasta `indexacao e busca/indexacao e busca.ipynb`

#### Quarta etapa:
Etapa de avaliação dos resultados da busca mostrada no notebook `indexacao e busca/avaliacao.ipynb`.