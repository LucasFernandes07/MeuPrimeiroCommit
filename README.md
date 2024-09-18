Git - Comandos Básicos
O Git é uma ferramenta de controle de versão distribuída que permite o acompanhamento de alterações de código, colaboração e gerenciamento de projetos. Abaixo estão os principais comandos para começar a usá-lo.

Configuração Inicial
Antes de utilizar o Git, é necessário configurá-lo com suas informações pessoais. Isso pode ser feito com os seguintes comandos:

bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"
Esses comandos definem o nome e o e-mail do usuário para todos os repositórios em sua máquina. Para configurar apenas um repositório específico, omita a flag --global.

Clonando um Repositório
Para clonar um repositório remoto (por exemplo, do GitHub) para o seu ambiente local, use:

bash
git clone https://github.com/usuario/repo.git
Isso irá copiar todos os arquivos e o histórico do repositório para o seu computador.

Verificando o Status do Repositório
O comando a seguir exibe o status dos arquivos no repositório, mostrando quais arquivos foram modificados, adicionados ou ainda não estão rastreados pelo Git:

bash
git status
Adicionando Arquivos
Antes de fazer o commit, é necessário adicionar os arquivos que foram modificados ao "stage" (área de preparação). Para isso:

Para adicionar um arquivo específico:

bash
git add nome-do-arquivo
Para adicionar todos os arquivos modificados:

bash
git add .
Commitando Alterações
O comando commit salva as alterações no repositório local. Sempre adicione uma mensagem descritiva para o commit:

bash
git commit -m "Mensagem do commit explicando as alterações"
Enviando Alterações para o Repositório Remoto
Após fazer o commit local, você pode enviar as mudanças para o repositório remoto (como GitHub, GitLab, etc.) usando:

bash
git push origin nome-da-branch
Substitua nome-da-branch pela branch que você está utilizando (geralmente main ou master).

Baixando Alterações do Repositório Remoto
Para manter seu repositório local atualizado com as últimas mudanças do repositório remoto, use:

bash
git pull
Isso baixa e mescla as alterações.

Criando e Trocando de Branch
Para criar uma nova branch e já mudar para ela:

bash
git checkout -b nome-da-branch
Para trocar para uma branch existente:

bash
git checkout nome-da-branch
Mesclando Branches
Para mesclar as alterações de uma branch (por exemplo, feature-branch) na branch atual (geralmente main):

bash
git merge nome-da-branch
Verificando Histórico de Commits
Para visualizar o histórico de commits e suas mensagens:

bash
git log
Esses são os principais comandos que cobrem a maioria das operações cotidianas com o Git.