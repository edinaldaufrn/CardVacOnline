#Aqui é o Dicionário de Dados do CardVacOnline
o Dicionário de Dados é um documento usado para armazenar informações sobre o conteúdo, formato e a estrutura de um
Banco de Dados, assim como os relacionamentos entre os seus elementos.
É importante manter um Dicionário de Dados para limitar erros ao criar a estrutura física do Banco de Dados no Computador.
Ele também é chamando de Repositório de Meta Dados.
Ele pode ser feito em forma de tabela as tabelas os atributos e os metodos.

##### D i c i o n a r i o
##DIcionario
 Tabela           Relacionamento            Tipo de Relacionamento      Descrição
CartaoSUS    usuario, enfermeira, vacina      cadastro, controle       para cadastrar as vacinas dos usuario do carto SUS
                                                cadastrar enfermeira, e usuario e as vacinas
                                                                   
Ususario      vacina, cartaoSUS                  cadstro               para cadastrar os usuarios di cartaoSUS
Vacina       usuario, enfermeira, vacina        aplicada, pendente     informa as vacinas aplicadas e pendentes
Enfermeira   cartaoSUS, vacina                  cadastro               Tabela para cadastro
--------------
T     abela
----------
casa | padaria | escola
-|-|-
cazinha| padaria| lapis
### Use o HTML que resolve a tabela como o excel
<table border="5">
    <tr>
        <td>Nome</td>
        <td>Idade</td>
        <td>Profissão </td>
    </tr>
    <tr>
        <td>Ted</td>
        <td>22</td>
        <td>Estudante</td>
    </tr>
    <tr >
        <td>Ralf</td>
        <td>26</td>
        <td>Designer</td>
    </tr>
</table>
