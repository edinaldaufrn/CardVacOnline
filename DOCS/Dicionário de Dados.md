# Dicionário de Dados do CardVacOnline
#### O Dicionário de Dados é um documento usado para armazenar informações sobre o conteúdo, formato e a estrutura de um
#### Banco de Dados, assim como os relacionamentos entre os seus elementos.
#### É importante manter um Dicionário de Dados para limitar erros ao criar a estrutura física do Banco de Dados no Computador.
#### Ele também é chamando de Repositório de Meta Dados.
#### Ele pode ser feito em forma de tabela as tabelas os atributos e os metodos.

### Dicionário de Dados Modelo Relacional

<table border="2">
    <tr>
        <th>Tabela</th>
        <th>Relacionamento</th>
        <th>Tipo de Relacionamento</th>
        <th>Descrição</th>
    </tr>
    <tr>
        <td>CartaoSUS</td>
        <td>Usuário, Enfermeira, Vacina</td>
        <td>Cadastro, Controle</td>
        <td>Tabela para cadastrar as vacinas dos usuários do cartão SUS, cadastrar usuário, enfermeira e também as vacinas.</td>
    </tr>
    <tr >
        <td>Usuario</td>
        <td>Vacina, CartaoSUS</td>
        <td>Cadastro</td>
        <td>Tabela para cadastrar os usuários do cartão SUS</td>
    </tr>
    <tr >
        <td>Vacina</td>
        <td>Usuario, Enfermeira, Vacina</td>
        <td>Aplicada, Pendente</td>
        <td>A tabela informa as vacinas aplicadas e pendentes</td>
    </tr>
    <tr >
        <td>Enfermeira</td>
        <td>CartaoSUS Vacina</td>
        <td>Cadastro</td>
        <td>Tabela para cadastrar as enfermeiras</td>
    </tr>
</table>

### Dicionário de Dados: Tabela Usuário

<table border="2">
    <tr>
        <th>Nome da Coluna</th>
        <th>Tipo de Dado</th>
        <th>Comprimento</th>
        <th>Restrinções</th>
        <th>Valor Padrão</th>
        <th>Descrição</th>
    </tr>
    <tr>
        <td>CPF</td>
        <td>long Int</td>
        <td>24 bytes</td>
        <td>Pk, NOT NULL</td>
        <td>N/D</td>
        <td>Número do CPF do Usuário</td>
    </tr>
    <tr>
        <td>Nome</td>
        <td>Caracteres</td>
        <td>80 Bytes</td>
        <td>NOT NULL</td>
        <td>N/D</td>
        <td>Nome do us</td>
    </tr>
    <tr>
        <td>Fone</td>
        <td>int</td>
        <td>16 bytes</td>
        <td></td>
        <td>N/D</td>
        <td>Fone para contato</td>
    </tr>
    <tr>
        <td>E-mail</td>
        <td>Caracteres</td>
        <td>40 bytes</td>
        <td></td>
        <td>N/D</td>
        <td>e-mail para contato</td>
    </tr>
    <tr>
        <td>Nº Cartao SUS</td>
        <td>Long int</td>
        <td>16 Bytes</td>
        <td>Fk</td>
        <td>N/D</td>
        <td>Nº do cartão do SUS</td>
    </tr>
</table>

#### Total de Dados para cada Registro: 160 Bytes

### Dicionário de Dados: Tabela para Vacina

<table border="2">
    <tr>
        <th>Nome da Coluna</th>
        <th>Tipo de Dado</th>
        <th>Comprimento</th>
        <th>Restrinções</th>
        <th>Valor Padrão</th>
        <th>Descrição</th>
    </tr>
    <tr>
        <td>Data</td>
        <td>Data</td>
        <td>8 Bytes</td>
        <td>NOT NULL</td>
        <td>N/D</td>
        <td>Data da aplicação da vacina</td>
    </tr>
    <tr>
        <td>Nome</td>
        <td>Caracteres</td>
        <td>80 Bytes</td>
        <td>NOT NULL</td>
        <td>N/D</td>
        <td>Nome da vacina</td>
    </tr>
    <tr>
        <td>Codigo</td>
        <td>int</td>
        <td>16 Bytes</td>
        <td>PK, NOT NULL</td>
        <td>N/D</td>
        <td>Código gereado Altomaticamente</td>
    </tr>
    <tr>        
        <td>Pendente</td>
        <td>Caracteres</td>
        <td>40 Bytes</td>
        <td></td>
        <td>N/D</td>
        <td>Data de vacina pendente</td>
    </tr>
    <tr>
        <td>COREN</td>
        <td>int</td>
        <td>8 Bytes</td>
        <td>FK</td>
        <td>N/D</td>
        <td>Codigo do enfermeiro</td>
    </tr>
    <tr>
        <td>NºCartaoSUS</td>
        <td>long int</td>
        <td>16 Bytes</td>
        <td>FK</td>
        <td>N/D</td>
        <td>Número do Cartão do SUS</td>
    </tr>
    <tr>
        <td>CPF Usuario</td>
        <td>lon int</td>
        <td>16 Bytes</td>
        <td>FK</td>
        <td>N/D</td>
        <td>Número do CPF do Usuário</td>
    </tr>
</table>

#### Total de Dados para cada Registro: 144 Bytes

### Dicionário de Dados: Tabela para Enfermeira

<table border="2">
    <tr>
        <th>Nome da Coluna</th>
        <th>Tipo de Dado</th>
        <th>Comprimento</th>
        <th>Restrinções</th>
        <th>Valor Padrão</th>
        <th>Descrição</th>
    </tr>
    <tr>
        <td>COREN</td>
        <td>int</td>
        <td>16 Bytes</td>
        <td>PK, NOT NULL</td>
        <td>N/D</td>
        <td>Código de enfermeira</td>
    </tr>
    <tr>
        <td>Nome</td>
        <td>Caracteres</td>
        <td>80 Bytes</td>
        <td>NOT NULL</td>
        <td>N/D</td>
        <td>Nome da vacina</td>
    </tr>
    <tr>
        <td>E-mail</td>
        <td>Caracteres</td>
        <td>40 Bytes</td>
        <td></td>
        <td>N/D</td>
        <td>E-mail para contato</td>
    </tr>
    <tr>
        <td>Fone</td>
        <td>lon int</td>
        <td>16 Bytes</td>
        <td>NOT NULL</td>
        <td></td>
        <td>Fone para contato</td>
    </tr>
</table>

#### Total de Dados para cada Registro: 152 Bytes

### Dicionário de Dados: Tabela para EnfermeiraSUS

 <table border="2">
    <tr>
        <th>Nome da Coluna</th>
        <th>Tipo de Dado</th>
        <th>Comprimento</th>
        <th>Restrinções</th>
        <th>Valor Padrão</th>
        <th>Descrição</th>
    </tr>
    <tr>
        <td>COREN</td>
        <td>int</td>
        <td>16 Bytes</td>
        <td>PK, FK</td>
        <td>N/D</td>
        <td>Código de enfermeira</td>
    </tr>
    <tr>
        <td>CartaoSUS</td>
        <td>log int</td>
        <td>16 Bytes</td>
        <td>PK, FK</td>
        <td>N/D</td>
        <td>Número do Cartão do SUS</td>
    </tr>
</table>

#### Total de Dados para cada Registro: 24 Bytes
