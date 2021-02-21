# Aqui é o Dicionário de Dados do CardVacOnline
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
        <td>Aplicada, Pendencia</td>
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
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
    </tr>
    <tr>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
    </tr>
    <tr>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
    </tr>
    <tr>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
    </tr>
    <tr>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
    </tr>
    <tr>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
    </tr>
    <tr>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
    </tr>
    <tr>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
    </tr>
</table>

### Dicionário de Dados Modelo Entidade Relacionamento para Vacina

### Dicionário de Dados Modelo Entidade Relacionamento para Enfermeira

### Dicionário de Dados Modelo Entidade Relacionamento para EnfermeiraSUS
