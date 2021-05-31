# Comandos Iniciais

Criar um repositório 
    
    git init

Criar um repositório Git sem uma cópia dos arquivos 

    git init --bare
    
Analisar o estado do repositório
        
    git status

Adicionar arquivos para serem commitados

    git add <nome_arquivo>

Commitar arquivos

    git commit -m "mensagem de identificacao do commit"

# Histórico de commits

oneline
    
    git log --online

verificar alterações        

    git log -p
    
# Log com parametros de formatação

    git log --pretty="parametros de formatação"
            
Retorna apenas os hash
    
    git log --pretty="format:%H"

Retorna hash resumido seguido pela mensagem do commit

    git log --pretty="format:%h %s"
        
# Repositório remoto
    
lista repositório remoto

    git remote

lista de repositórios + caminhos
        
    git remote -v

adicionar repositório remoto

    git remote add <nome> {caminho}
    
remover um repositorio remoto

    git remote remove <nomeDoRepositório>

clonar um repositório

    git clone {caminho} 
    
# Merge e Rebase

Merge: Gera sempre um novo commit informando que houve uma mescla entre 2 branchs
    
    git merge

rebase: traz os commits de uma branch para outra (não gera commit, simplificando log)

    git rebase

Visulualize usando diagramas de ramifiucações detalhadas (Site bacana)

    https://git-school.github.io/visualizing-git/

Artigo: Git - Rebase vs Merge

    https://medium.com/datadriveninvestor/git-rebase-vs-merge-cc5199edd77c

# Desfazer

Desfazer uma alteração antes de adiciona-lá
    
    git checkout -- <nome_do_arquivo>

Desfazer uma alteração após adiciona-lá

    git reset HEAD <nome_do_arquivo>

    git checkout --<nome_do_arquivo>

Desfazer uma alteração já commitada

    git revert <id_commit>

Deixar um código no estado de um commit 

    git checkout <hash_commit>


# Commit temporário

Guardar um trabalho para retomá-lo posteriormente

    git stash

Visualizar quais alterações estão na stash

    git stash list

Aplicar uma alteração específica da stash    

    git stash apply <numero>

Remover um determinado item da lista de stash

    git stash drop <numero>

Aplica e remove a última alteração que foi adicionada na stash

    git stash pop

