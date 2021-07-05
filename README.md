# Pentaho_GetEmail
Exemplo de rotina para se conectar em uma conta de email, filtrar um determinado email, salvar o email e os anexos e em seguida Transformar e Carregar dados em outro arquivo ou banco de dados. 
Para simplificar o exemplo, eu simplesmente gerei um arquivo txt com os dados coletados a partir do CVS anexado ao email, mas poderia ser feito um insert/update em um banco de dados.

# Rotina completa
![image](https://user-images.githubusercontent.com/79167966/124199548-8162dc00-daa9-11eb-87a4-0d3c8488ff30.png)

# Step Get emails from POP3/IMAP
Aqui eu fiz a autenticação usando IMAP e em seguida optei por salvar apenas o anexo em uma determinada pasta. 

![image](https://user-images.githubusercontent.com/79167966/124199988-a015a280-daaa-11eb-98aa-ebf4167cb241.png)

# Configurações de pasta a ações
Aqui informo que quero pegar os emails que se enquadrarem no filtro que irei informar e qual pasta deseja acessar, no exemplo INBOX. 

![image](https://user-images.githubusercontent.com/79167966/124200100-e2d77a80-daaa-11eb-8a43-ec49dfded64d.png)

# Filtros
Aqui é feito o filtro para selecionar determinadas mensagens de um determinado remetente  e assunto.

![image](https://user-images.githubusercontent.com/79167966/124200197-17e3cd00-daab-11eb-8532-9e0ac161546a.png)

Esse step faz a conexão, filtro e a ação solicitada, no exemplo é baixado o anexo e salvo em uma pasta. Em seguida a JOB aciona uma transformação que faz a leitura do arquivo e gera um txt contendo os dados coletados. 


