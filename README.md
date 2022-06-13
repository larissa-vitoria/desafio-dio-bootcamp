# Anotações sobre a aula introdutória ao uso do Git/GitHub - Uso em sistema operacional Windows :pencil:

## Comandos básicos no terminal de comando:

- cd (change directory) - acessa e muda o diretório atual
- dir (directory) - exibe os arquivos do diretório
- mkdir (make directory) - cria um novo diretório
- del (delete)/ rmdir (remove directory) - remove um diretório

## Comandos principais do terminal do GitBash:

- git init - inicia um repositório git no diretório
- git status - exibe o status dos arquivos
- git add - adiciona o arquivo indicado ao stage
- git add. - adiciona todos os arquivos ao stage
- ls - exibe os arquivos existentes no diretório. A flag -a exibe arquivos ocultos, incluindo o .git
- mv - move o arquivo para outro repositório
- .. - volta/sobe um nível
- commit - valida e salva as mudanças feitas e envia para o estágio não modificado, com uma mensagem. Faz um "snapshot" 
- commit -m: a flag m adiciona uma mensagem
- git config --list: lista as configurações globais do git na máquina
- git config --global --unset <propriedade>: remove um atributo das configurações
- git remote add origin <link>: adiciona a origem (destino remoto) para a qual os arquivos serão enviados
- git remote -v: lista as listas de repositório cadastradas
- git push origin master (é a branch) - envia o arquivo para a origem
- git push - envia o arquivo do repositório local para o remoto

## Objetos Internos do Git:

- Blobs (Binary Large Object) - tipo de objeto que armazena cada arquivo do repositório
- Trees - Objeto que arquiva pastas e pode apontar para outras árvores (trees). É um conjunto de valores de índices.
- Commit - Armazena os "snapshots" do projeto com metadados do autor e data das modificações, possibilitando acessar as versões da alteração

## Chave SSH e Token :closed_lock_with_key::

- A Chave SSH representa uma chave pública e uma privada. A pública é postada no Git. A chave privada é específica para a máquina e o usuário. 
- O Token substitui a senha de acesso, e pode ser utilizado pelo mesmo usuário em diferentes máquinas.

Obs: Ambos são usados por questões de segurança, para impedir que ações sejam feitas no projeto sem o conhecimento ou permissão do autor.

