Comandos 

    # criar um repositório 
    
        git init

        # ciar um repositório Git sem uma cópia dos arquivos 

        git init --bare
    
    # analisar o estado do repositório
        
        git status

    # adicionar arquivos para serem commitados

        git add <nome_arquivo>

    # commitar arquivos,

        git commit -m "mensagem de identificacao do commit"

    # verificar o histórico de commits

        git log --online
        
        git log -p
        
        git log --pretty="parametros de formatação"
            
        # Retorna apenas os hash
            git log --pretty="format:%H"

        # Retorna hash resumido seguido pela mensagem do commit
            git log --pretty="format:%h %s"
        
    
    # listar repositórios remotos

        git remote

    # lista repositórios e caminhos
        
        git remote -v

    # adicionar repositório remoto

        git remote add <nome> {caminho}
    
    # remover um repositorio remoto

        git remote remove <nomeDoRepositório>

    # clonar um repositório

        git clone {caminho} 
    
