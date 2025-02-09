
### ERRO 1: Data de Nascimento Apresentada de Forma Incorreta
**Funcionalidade:** Cadastro de Usuário
- **Cenário:** Data de nascimento exibida incorretamente
    - *Dado* que estou na página de cadastro de usuários
    - *Quando* insiro a data de nascimento "15/03/1990"
    - *Então* a data exibida na interface deve ser "15/03/1990"
    - *Mas* a data exibida é "07/02/2025"

<img src="assets/imagem - Data setada para o dia 07-02-2025.png" alt="Data incorreta">

<br>

### Erro 2: Botão de Edição Não Funciona
**Funcionalidade:** Edição de Usuário
- **Cenário:** Botão de edição não funciona
    - *Dado* que estou na lista de usuários cadastrados
    - *Quando* clico no botão "Editar" ao lado de um usuário
    - *Então* a interface deve permitir a edição das informações do usuário
    - *Mas* nenhuma ação é realizada ao clicar no botão

<img src="assets/imagem - Erro na edição.png" alt="Botão de edição não funciona">

<br>

### Erro 3: Botão de Deletar Não Funciona Corretamente
**Funcionalidade:** Deleção de Usuário
- **Cenário:** Botão de deletar não remove o usuário
    - *Dado* que estou na lista de usuários cadastrados
    - *Quando* clico no botão "Deletar" ao lado de um usuário
    - *Então* o usuário deve ser removido da lista
    - *Mas* o usuário permanece na lista, embora uma mensagem de deleção seja exibida

<img src="assets/imagem - Erro na exclusão 1.png" alt="Mensagem que aparece na deleção">
<img src="assets/imagem - Erro na exclusão 2.png" alt="Após a mensagem">

<br>

### Erro 4: Mensagem de Campo Obrigatório Fecha Janela de Cadastro
**Funcionalidade:** Cadastro de Usuário
- **Cenário:** Mensagem de campo obrigatório fecha janela de cadastro
    - *Dado* que estou na página de cadastro de usuários
    - *Quando* deixo o campo "Empresa" em branco
    - *E* clico no botão "Salvar"
    - *Então* a interface deve exibir uma mensagem de erro e manter a janela de cadastro aberta
    - *Mas* a interface exibe a mensagem de erro e fecha a janela de cadastro

<img src="assets/imagem - Aviso preenchimento de empresa fecha a janela toda.png" alt="Formulário fecha sozinho">

<br>

### Erro 5: Validação de Número de Telefone e E-mail
**Funcionalidade:** Cadastro de Usuário
- **Cenário:** Validação de número de telefone e e-mail inválidos
    - *Dado* que estou na página de cadastro de usuários
    - *Quando* insiro um número de telefone inválido "12345"
    - *E* insiro um e-mail inválido
    - *E* clico no botão "Salvar"
    - *Então* a interface deve exibir mensagens de erro para os campos inválidos
    - *Mas* a interface permite o cadastro com dados inválidos

<img src="assets/imagem - Email inválido inserido.png" alt="Email inválido cadastrado">
<img src="assets/imagem - Telefone inválido inserido.png" alt="Telefone inválido cadastrado">

<br>

### Erro 6: Telefone Obrigatório Não Validado
**Funcionalidade:** Cadastro de Usuário
- **Cenário:** Telefone obrigatório não é validado
    - *Dado* que estou na página de cadastro de usuários
    - *Quando* deixo o campo "Telefone" em branco
    - *E* clico no botão "Salvar"
    - *Então* a interface deve exibir uma mensagem de erro informando que o telefone é obrigatório
    - *Mas* o sistema permite que o registro seja salvo sem o número de telefone

<img src="assets/imagem - Dado obrigatório não solicitado.png" alt="Dado obrigatório não solicitado como obrigatório">