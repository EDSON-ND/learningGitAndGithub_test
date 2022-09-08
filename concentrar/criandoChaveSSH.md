# PRIMEIROS PASSOS NO GIT
### 2) CRIANDO CHAVES SSH

   1. No Git bash digite: 
  *"ssh-keygen -t ed_25519 -C **digite seu email cadastrado no GitHub**"
	2. Em seguida, precisaremos da chave pública para inseri-las no GitHub. Para ter acesso a ela, navegue até a pasta **.ssh**, e digite o comando **LS**;
	3.  O resultado serão dois arquivos, um deles será a chave pública que terminará com *.pub*, anote-a;
	4.  No Git, digite:
*"CAT ID_ED25519.pub"*;
	5. Logo em seguida, o sistema apresentará uma sequência que deverá ser copiada, e colada na página de configurações SSH do Git Hub;
	6. Após é necessário inicializar o serviço **SSH agent**, para tanto digite:
 *"eval $(ssh-agent -s)"*;
	7. Por fim, a chave privada deve ser adicionada por meio do comando **SSH-ADD**:
*"ssh-add <passar o caminho onde a chave está>"*
**obs.: caso tenha digitado alguma senha no momento em que criou a chave ssh, deverá digitá-lá;**
 
