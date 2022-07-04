### Semana 1 - Dia 25/05/2022 - Aulas 001a004 - Atividade Supervisionada


1. Elaborar uma pesquisa sobre o tema "_Rest API_".
2. Elaborar um texto de pelo menos uma página, descrito com suas próprias palavras, destacando:
* As definições dos conceitos envolvidos;
* As principais características deste conceito (pelo menos umas cinco).

INSTRUÇÕES:
1. Este é um arquivo no formato _markdown_ (.md), caso você precise de orientações a respeito da forma como editar este tipo de arquivo, acesso este [link](https://guides.github.com/features/mastering-markdown/);
2. Edite este arquivo adicionando o texto, conforme especificado;
3. Remova esta Seção de INSTRUÇÕES, do arquivo respondido.
6. Faça o _Commit_ do arquivo atualizado com suas respostas, no seus repositório cs-2022-1, na pasta aula01.
7. Isso deve ser feito até as 23h59min do dia 27/05/2022.


### API REST

Uma API é uma "aplicação de interface de programação", utilizada para a transmisão de dados entre o lado servidor e o lado cliente. 
REST é o acrônimo para, na tradução, "Transferência de Estado Representacional", e foi concebido por Roy Thomas Fielding em 2000 sendo uma arquitetura
de transferência de dados para a web como uma alternativa ao protocolo mais utilizado até então, o SOAP (Protocolo Simples de Acesso a Objetos). Por utilizar de um estrutura rígida
e baseada na linguagem de marcação XML, o protocolo SOAP apresentava problemas de desempenho. A arquitetura REST, possibilitou a padronização da transmissão de dados através da introdução de
limitações de interface às quais as aplicações devem obedecer sendo elas um protocolo sem estado, onde cada mensagem HTTP contém todas informações necessárias para a comunicação cliente-servidor, sem a
necessidade de persistência desses dados, a sintaxe universal que permita identificar os recursos, utilizando-se da URI, o uso de hipermídia para tramissão dos dados, sendo os
mais utilizados o HTTP, XML e JSON, mas com suporte a vários outros, e um conjunto limitado e definido de operações, que se dá pelas operações de POST (envio de informações ao servidor), 
GET(obtenção de informações do servidor), PUT (atualização de informações do servidor) e DELETE (remoção de informações do servidor), dentre outros.
A utilização desses limitadores simplificou a forma que a comunicação cliente servidor é feita e possibilitou uma melhoria no desempenho da transmição de dados.
A arquitetura REST permite que as APIs, independentemente da linguagem que tenha sido criada, possa se comunicar com qualquer aplicação via HTTP, podendo a aplicação cliente
tratar e manipular os dados da forma que melhor entender.