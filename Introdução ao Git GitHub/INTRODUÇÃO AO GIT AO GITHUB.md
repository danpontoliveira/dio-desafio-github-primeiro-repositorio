**INTRODUÇÃO AO GIT AO GITHUB**

**(Repositório de código)**

*\*Software não é feito sozinho, mas sim de forma colaborativa Ex.(Linux).*

***BENEFÍCIOS***

*1 – Controle de Versão*

*2- Armazenamento em nuvem*

*3 – Trabalho em equipe*

*4 – Melhorar seu Código*

*5 - Reconhecimento*

***COMANDOS BASICOS E NAVEGAÇÃO***

- ` `*Mudar de pasta*
- *Listar as pastas*
- *Criar pasta/arquivos*
- *Deletar pasta/arquivos*

` `*- Windows – CMD – comando (**dir+enter**)*

*Aparecerá a lista de diretórios do Windows*

*Linus – (**Ls+enter**)*

` `*- (**cd** /) – entrar nas pastas*

*(**Cd** Windows)*

*(**dir**) – todos os arquivos e pastas executáveis dentro desta pasta.*

*Para voltar – retroceder um nível (**cd**..)*

*Para limpar o terminal (**cls**)*

*\*Tab autocompleta o comando (atalho).*

***CRIAR PASTA -**  (**mkdir**) e nome da pasta = mkdir workspace*

*(**dir**) mostra os diretórios da pasta criada.*

*(**Cls**) – para limpar*

*(**cd** **wo+tab**) para completar o workspace*

*(**echo** **>** **hello.txt**) >direcionar*

***PARA DELETAR***

*(**del** **workspace**)*

*\*Porém, há uma diferença entre deletar arquivos e deletar repositório, esse comando só deleta os arquivos dentro do repositório.*

***ATALHO PARA NAVEGAR ENTRE O HISTORICOS DE COMANDOS***

***(seta para cima) acessar o texto para criar o arquivo***

***-Listar***

***-Retornar***

***-Limpar***

***Para remover o repositório usar o comando (rmdir workspace /S /Q).***

***REALIZANDO INSTALAÇÃO DO GIT:***

[Git - Downloads (git-scm.com)](https://git-scm.com/downloads)

-Assegurar que os check-box estejam marcados:

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.001.png)

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.002.png)

Windows:

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.003.png)

Linux/Mac:

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.004.png)

**COMO O GIT FUNCIONA POR DEBAIXO DOS PANOS:**

-SHA1 – Secure Hash Agorithm (Algoritmo de Hash seguro) \* encriptação.

-Objetos fundamentais

-Sistema distribuído

-Segurança

\*A encriptação gera conjunto de characters identificador de 40 dígitos.

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.005.png)

Ex. utilizando no Desktop, clicar com o botão direito e abrir o ‘gitbash here’

(openssl sha1 nome do arquivo.txt)

Chave ex. criado: 80c625a2d975956uucbcc7c28017f27b66f0e69


Qualquer alteração no arquivo, altera o código de identificação (chave).

**OBJETOS FUNDAMENTAIS:**

- BLOBS
- TREES
- COMMITS

**\*BLOBS**:

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.006.png)

***\*\****

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.007.png)

*Para que a chave continue a mesma:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.008.png)

***\*TREE**:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.009.png)

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.010.png)

***COMMIT**:*

*(Mais importante)*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.011.png)

*- Forma segura de demonstrar que o arquivo, foi inalterado, pois toda alteração gera uma nova chave (garante a autenticidade).*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.012.png)

*\*Sistema Distribuído Seguro\**


***CHAVES SSH E TOKENS:***

*CHAVE SSH –* 

*- Entrar no Github  - Settings – Chave SSH Keys*

*-  Entrar no Git bash (maquina) e seguir a sequencia de comandos:*

*(ssh-keygen -t ed25519 -C e-mail usando no github)*

(/c/Users/Dani/.ssh/id\_ed25519):

Cadastrar senha: xxxx0x0x0x

SHA256:0000000xxx0x0x0x0x0x0x0x0x0xx+/0x0x0x xxxxx@e-mail.com

The key's randomart image is:

+--[ED25519 256]--+

|   o===\*\*+..     |

|  .. o=\*=\*=o     |

|    . o=\*+B.+    |

|   o . +.B.  o   |

|  . . o S o .    |

|     .     o     |

|      E   . .    |

|     .  .o . .   |

|      o+. . ...  |

+----[SHA256]-----+

*Localizar as chaves pública e privada*

*(cd /c/Users/Dani/.ssh/)*

*(cat* id\_ed25519.pub)

Chave pública – salvar no GitHub

ssh-ed25519 0000000xxx0x0x0x0x0x0x0x0x0xx+/0x0x0x <xxxxx@e-mail.com>

*- (ls) no git bash – para verificar aonde esta*

*- (pwd) mostra o caminho completo*

*- (*eval $(ssh-agent -s) – para criar o agente pid ‘1219”

*- (*ls) 

*- (*ssh-add id\_25519) – passar para o agente a chave privada, após digitar a senha

\*Clonar o code pelo SSH

(git clone) colar o link ssh.

**CONFIGURAR UMA CHAVE PARA ACESSO REMOTO**

Token de acesso Pessoal:

**gfg\_qK3Dc8Kcc3aB500f5d85ffcffksOJCJ6ukHNf00AeV0h1**

\- Para criar, **settings** – **Developer** **settings** – **Personal** **Acess** **tokens** – **generate** **new** **token**, pode inserir um prazo para expirar – opção **repo** (atende) – **generate** **token**

Pode ser usando o url em HTTPS, para clonar

\*\*Passo a passo se aplica para maquinas que não sejam de confiança, se é máquina é sua, o passo anterior atende.

**PRIMEIROS COMANDOS COM O GIT**

-Iniciar o GIT

-Iniciar o versionamento

-Criar um commit

Início dos códigos

- \*Git init
- \*Git add
- \*Git commit

\- Abrir a pasta workspace criada pelo git bash, abrindo a pasta c: do Windows, clicando com o botão do direto já vai direto para o repositório da pasta:

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.013.png)

Após criar a pasta lista-receitas, dentro da workspace

(git init) – o comando (ls) não vai lista a pasta, pois ela é oculta para os códigos-

O comando a ser usando é o (ls -a):

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.014.png)

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.015.png)

*Voltar com o (c ..), limpar (crt+l)*

*Configuração inicial necessária:*

(git config --global user.email <e-mail@e-mail.com>)

(git config --global user.name [dsoliveira](mailto:danpontoliveira@gmail.com))


*- **Adicionado um arquivo**:*

*Markdown*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.016.png)

*Baixar o app Typora (leitor de Markdown)*

*# espaço e o titulo*

*(: escrever o emoticon, é possível inserir*

*Criar \* espaço-1 espaço*

*-Após formatar o arquivo, necessário commitar com os dados infra:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.017.png)

*Resultado com sucesso:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.018.png)

***CICLO DE VIDA DOS ARQUIVOS DENTRO GIT***

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.019.png)

*COMMIT- move os arquivos do staging para unmodified*

*\*tudo que está no repositório tem que estar commitado, para constar no repositório remoto (GitHub).*

*\*\*Comando no Git para verificar status dos arquivos, se estar untraking, unmodified, etc..*

*(git status):*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.020.png)

*------*

*(mkdir nome da pasta “receitas”) – criando outra pasta*

*(mv nome da pasta.md ./a pasta para qual deseja mover/ “Strogonoff.md ./receitas/”) – para mover a pasta:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.021.png)

*- Quando não localiza:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.022.png)

*\*\**

*-Movendo a pasta e commitando: ![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.023.png)*

*-O Comando (git add \*), adiciona todos as modificações para a stage (anterior ao palco, ‘entrar em ação’) ![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.024.png)*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.025.png)

***TRABALHANDO COM O GITHUB:***

*-Verificar se as informações no Git estão iguais ao GitHub para fácil comunicação entre eles*

*(git config –list)*

*\*Se necessário alterar usar o comando (git config –global –unset user.name “o que precisa ser corrigido”)*

*\*\*Pata configurar após apagar, basta utilizar o mesmo código, sem o “unset” (git config –global user.name “o que precisa ser corrigido”)*

*Ex.:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.026.png)

*ADICIONANDO REPOSITÓRIO*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.027.png)

*-Neste caso em especifico, deixaremos o “README” desmarcado, pois já adicionamos no repositório local:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.028.png)

*-Copiar o URL para inserir no repositório local:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.029.png)

*-Código no Git para adicionar ao repositório remoto:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.030.png)

*Traz a lista de repositórios cadastrados:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.031.png)

*\*\*“origin” é apenas um alias(apelido) por convenção para não ter que ficar digitando a url novamente,*

*- Agora iniciar o push, para empurrar o código:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.032.png)

*- Autenticar no GitHub:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.033.png)

*\*\*O GitHub sempre irá procurar um arquivo markdown*

***RESOLVENDO CONFLITOS:***

***(conflitos de merge)***

*Passo a Passo para alterar o arquivo readme.md e atualizar no GitHub:*

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.034.png)

*\*Código para puxar a versão do GitHub e comparar ambas:*

*(*git pull origin master)

Após verificar qual esta certo e atualizada:

*(*git commit -m “resolve conflitos”)

Após resolver conflito e commitar, enviar novamente ao repositório:

*(*git push origin master)

**CRIANDO LINK NO GITHUB:**

![](Aspose.Words.2c1dc970-d351-4081-b756-c2a0a4616ae6.035.png)



