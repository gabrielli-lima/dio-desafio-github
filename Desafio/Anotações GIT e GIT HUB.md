# Anotações GIT e GIT HUB

- **Comandos básicos**
    
    ### GUI x CLI
    
    cli → comand line interface
    
    comando diferentes no windows e linux/apple(unix)
    
    bash terminal do linux
    
    **windows**
    
    **dir** (Win) =
    
    **cd** → base do diretório c
    
    cd windows
    
    **cd ..**     -> retroceder 1 nível
    
    **cls** =
    
    **mk dir** workspace = nos dois (W e L)
    
    **echo hello > hello.txt** → cria uma pasta com um arquivo txt escrito hello → é o mesmo nos dois
    
    **del** workspace → deleta arquivos e não um repositório
    
    **rmdir** workspace **/s /q** → excluir o repositório (em verde são duas **flags)**
    
    **linux**
    
    **ls** (linux)
    
    **cd etc**(etc é uma pasta que tem no linux)
    
    **clear** → para limpar o terminar ou crt + l no linux
    
    **sudo su** -> permissão para criar pasta
    
    **rm -rf** → **flags r** recursivamente/recursivo para excluir todas as pastas contidas dentro - **f** force para não aparecer nenhum tipo de confirmação
    
- **Tópicos fundamentais para entender o funcionamento do Git**
    - Sha1
        - Secure Hash Algorithm
        - Algoritmo de encriptação
        - Gera um conjunto de caracteres identificador de 40 dígitos
        - É uma forma curta de representar um arquivo
    - Objetos fundamentais
        
        **Blobs** → tem metadados, guarda o sha do arquivo(caractere identificador dele)→ aponta para diretórios que contem arquivos e aponta para arquivos também                 
        
        **Trees** → tem metadados, tem blobs, guarda o nome do arquivo→ pode apontar para outra árvore→ assim como um diretório pode ter um diretório
        
        **Commits**→ aponta para árvore, para parente(ultimo commit antes dele), aponta para um autor e mensagem
        
    - Sistema distribuído
        
        É um sistema distribuído seguro
        
        - Sistemas de pesquisas (motores de busca)
        - Sistemas financeiros
        - Jogos Online
        - Redes Sociais e plataformas idênticas
        
        Todos os sistemas apresentados anteriormente têm máquinas dispersas por todo o mundo, com acessos concorrentes e muitos desafios nos processos de comunicação (ex. hora do sistema – devido à distribuição geográfica, possíveis falhas de componentes, etc). A comunicação é simplesmente feita com base em mensagens
        
    
- **Chave SSH e Token**
    
    Chave SSH → forma de estabelecer uma conexão segura e encriptada entre duas maquinas
    
    Chave pública e privada
    
- **Iniciando o Git e criando um commit**
    
    **git init** → inicializar/cria um repositório
    
    não aprece a pasta pq é uma pasta oculta e gerencial do git é onde estão os códigos do git e onde ele versiona os objetos manipulados
    
    **ls -a →** para ver a página oculta
    
    Colocando nome no repositório 
    
    **git config --global user.email "gabrielli@email.com"**
    
    **git config --global user.name Gabi**
    
    Criando um commit
    
    **git add * →** adiciona as mudanças para a área de staging 
    
    **git commit -m "**commit inicial**”**
    
- **Passo a passo no ciclo de vida**
    
    tracked e untracked
    
    unmodified | modified | staged (se preparando para fazer parte de outro tipo de agrupamento)
    
    md→ arquivo markdown → HTML
    
    **git status**
    
    **mv** bolodeCenoura.md./receitas/ → movendo uma pasta
    
    **git add nomeArquivo →** adiciona arquivos novos ou alterados no diretório de trabalho à área de staging do Git
    
    **git add ***
    
    adiciona as modificações para a staging  área
    
    Criando um commit
    
    **git commit -m “**mensagem**”**
    
    **git push origin master →** envia os commits locais para o remoto
    
- **Conflitos que acontecem no GitHub e como resolvê-los**
    
    Quando dois arquivos estão editados na mesma linha gera um conflito, o que fazer:
    
    *Antes de dar um git push:
    
    1. **git pull orign master →** para atualizar a branch local de acordo com as branches remotas
    2. Editar o arquivo manualmente e escolher qual informação irá ocupar o lugar com o conflito
    3. **git add ***
    4. **git commit -m “”**
    5. **git push origin masters**
    
    Clonar o repositório via terminal (git bash)
    
    1. Link do repositório no git hub
    2. **git clone https://github.com/python/cpython.git**
    
    **git remote -v →** traz os repositórios remotos onde está sendo apontado