### Tarefa 003: Git Exercícios - 03/06/2021.

Responda as questões abaixo (exercite os comandos do git correspondentes). Lembre-se de que o “interessante” não é exatamente o conjunto de respostas, mas o processo de obtê-las e a experiência obtida com a execução dos comandos.


1. Qual o comando para obter a versão instalada do Git?
git --version

2. Qual o efeito da execução de cada um dos comandos abaixo?
  a. git help
Mostra operações básicas de git e suas definições.

  b. git help checkout
Mostra definição e opções para operação de checkout.

  c. git help merge
Mostra definição e opções para operação de  merge ("mescla").

  d. git init
Inicia um repositório git na pasta.

  e. git add --all
Adiciona todas as alterações do repositório no controle de versão local.

 f. git add -u
Atualiza a situação dos arquivos sem adiciona-los ao controle de versão.

  g. git config -l
Apresenta todas as variáveis de configuração do repositorio versionado.

  h. git mv a.txt b.txt
Renomeia o arquivo a.txt para b.txt

  i. git reset --hard
Retorna a versão para o commit apontado, apagando todas alterações pendentes e comitadas no intervalo, limpando a árvores de trabalho.

  j. git log -27
Lista os últimos 27 commits do repositório.

3. O fluxo “clássico” de interação com o Git é algo como “alterar um ou mais arquivos”, “acrescentar essas mudanças para serem contemplados no próximo commit” e, finalmente, executar um “commit”. Quais os comandos necessários para realizar os dois últimos “passos” desse fluxo?
git add .
git commit -m "mensagem de comit"

4. Qual o comando deve ser executado para identificar o que foi alterado desde o último “commit”?
git diff

5. Em um dado repositório, arquivos simplesmente copiados para lá, ou seja, _untracked_, podem ser exibidos/identificados com que comando?
git status

6. Qual o comando para efetuar um _commit_?
git commit 

7. Qual o comando que devemos empregar para descartar mudanças ocorridas no arquivo teste.txt, por exemplo?
git restore teste.txt

8. O que deve ser feito para que um determinado diretório do seu repositório seja ignorado pelo Git? Faça uma busca por **.gitignore**.
Adicionar uma entrada com a seguinte sintaxe no arquivo .gitignore: <nomeDoDiretorio/**>

9. O que acontece se o seu repositório local for acidentalmente removido?
Não há perda se os dados estiverem sincronizados com o repositório remoto.

10. Como clonar um repositório remoto?
git clone <endereçoRemoto>

11. Em alguns cenários **git log** pode produzir extensos resultados. Se houver interesse em visualizar o histórico de um repositório, onde cada mudança é fornecida exatamente em uma única linha, qual o comando que deve ser empregado?
git shortlog

12. Em qual arquivo o Git armazena informações de configuração empregadas por usuário?
No arquivo config dentro da pasta .git

13. Qual o comando para criar um repositório local?
git intit

14. Qual o nome do diretório criado pelo Git quando se executa o comando **git init**?
.git

15. Qual o comando para adicionar todos os arquivos modificados? (Aqueles para os quais **git status** identificam como **modified**?)
git add .

16. O Git faz uso do valor de hash conhecido por SHA1. O que isto significa? Qual o propósito? O que é SHA1?
SHA1 é um algoritmo de encriptação, o valor criado por este algoritmo identifica o commit ou operação realizada no repositório.

17. Qual a palavra para indicar o último _commit_ em vez do valor de hash SHA1 correspondente?
HEAD

18. Quando se cria dois arquivos usando um editor de texto qualquer e, na sequência, executamos o comando **git add -u**, os dois arquivos criados passam de _untracked_ para _new file_?
Não, git add -u apenas atualiza o status dos arquivos já preparados, ignorando arquivos novos.

19. Qual o efeito da execução dos dois comandos abaixo, nesta ordem, em um dado repositório?
**git reset --soft HEAD~1**
**git reset --hard**
O primeiro comando 'reseta', ou seja, desfaz as alterações já comitadas para o commit imediatamente anterior, mantendo a working tree e não alterando o índice já versionado..
O segundo comando apaga as alterações que agora estão na working tree, bem como desfaz as alterações feitas no índice.

20. Após o emprego de um ambiente integrado de desenvolvimento (IDE), é comum a criação de arquivos e diretórios. Qual o comando que podemos empregar para remover arquivos e diretórios _untracked_?
git clean -fd

21. Qual o nome do arquivo no qual podemos inserir a indicação para o Git de arquivos e diretórios a serem ignorados?
.gitignore

22. Quando se cria o arquivo _MinhaClasse.class_ em um dado diretório e desejamos que arquivos com a extensão .class, como neste caso, sejam ignorados por todos os membros de uma equipe que estão contribuindo com um dado projeto, como devemos proceder?
*.class

23. jQuery é uma famosa biblioteca em JavaScript. Consulte detalhes em [jQuery](http://jquery.com). O repositório correspondente encontra-se em [gitRep](https://github.com/jquery/jquery.git). Faça o clone deste repositório.
24. No repositório **jqueryrepo**, criado no passo anterior, qual o efeito do comando
**git shortlog -sne**?
Exibe o log de commits ordenado pelo número de commits de cada autor, exibindo o número de commits, o nome do autor e o email.

25. No repositório **jqueryrepo**, qual o efeito de **git remote -v**?
Mostra as URLs de fetch e push cadastradas no repositório.

26. Um repositório Git pode ser etiquetado ao longo do tempo. Ou seja, _commits_ específicos podem ser “marcados” ou “etiquetados” para facilitar referências posteriores. Para listar todas as “etiquetas” (_tags_) estabelecidas para um dado repositório, qual comando deve ser executado?
git tag -a <tag> -m <mensagem_da_tag>

27. Caso um dato repositório retorne muitas “marcas” ou “etiquetas” para o comando **git tag**, como retornar apenas aquelas que atendem a determinado padrão, por exemplo, iniciadas por 2.0?
git tag -l "2.0*"

28. Qual o efeito do comando **git tag -a 3.4-gold -m “minha versão ouro”**?
Cria uma tag
29. Após executado o comando acima, qual o efeito de **git show 3.4-gold**?
Mostra os detalhes da tag, como horário de criação e detalhes do último commit.

30. O que o comando **git push origin 3.4-gold** teria como efeito?
Faria o push do repostório no estado que se encotrava quando da criação da tag.

31. Após executar um commit, qual o efeito de **git commit --amend**?
Amend "corrige" o commit anterior, adicionando as alterações preparadas ao commit.

32. Após executar **git add x.txt**, qual o efeito de **git reset HEAD x.txt**?
Remove as alterações do  arquivo, devolvendo para a working tree.

33. Após alterar o conteúdo de um arquivo committed em passo anterior, qual o efeito do comando **git checkout -- a.txt**?
Restaura o arquivo ao estado anterior.

34. Qual a diferença entre os comandos **git reset HEAD a.txt** e **git checkout -- a.txt**?
O primeiro retorna o arquivo para o estado em HEAD, ou seja um commit ou estágio específico, o segundo restaura o arquivo conforme seu estado no índice.

35. Veja como interpretar o resultado de git diff [aqui](https://medium.com/therobinkim/how-to-read-a-git-diff-6c87a9dc47c5). Execute, em um dos seus projetos, o comando **git diff HEAD~1 HEAD** e certifique-se de que entende o resultado apresentado.
git diff, no terminal, mostra as adições em verde e as remoções em vermelho, em comparação com o arquivo original e/ou do último commit, separando cada arquivo e suas modificações com um hash próprio.


INSTRUÇÕES:

1. No seu repositório pessoal, criar a pasta aula04.
2. Commitar este arquivo respondido nesta pasta.
3. A data limite para concluir esta tarefa é dia 07/06/2021, as 23h59min.











</DIV/>
