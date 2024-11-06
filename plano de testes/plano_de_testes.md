# Especificação dos Casos de Teste

## 1. Caracterização do Caso de Teste

<p align = justify><b>Descrição:</b> Cada caso de teste representa uma situação particular ou uma funcionalidade específica do Sistema de Ordem de Serviço que deve ser analisada detalhadamente. Através desses testes, verifica-se o comportamento do sistema em diferentes cenários, garantindo que ele esteja executando corretamente as tarefas para as quais foi projetado. Essa abordagem é essencial para identificar possíveis erros ou falhas, permitindo que sejam feitos ajustes antes que o sistema seja utilizado em um ambiente de produção. Assim, os casos de teste são uma ferramenta importante para assegurar que o sistema atende aos requisitos definidos e funciona de acordo com as expectativas dos usuários.</p>

## 2. Especificação de Entradas, Resultados Esperados e Casos de Testes

<p align = justify><b>Descrição:</b> Esta seção abordará em detalhes as diferentes entradas que o sistema deverá processar, especificando os resultados esperados para cada uma dessas entradas ao serem analisadas. O objetivo é descrever como o sistema deve responder em cada situação prevista, garantindo que o comportamento seja conforme esperado. Para alcançar essa validação de forma eficiente, será aplicada a técnica de particionamento por classes de equivalência.</p>

<p align = justify> A técnica de particionamento por classes de equivalência, amplamente utilizada em testes de software, consiste em dividir o conjunto de possíveis entradas em classes de equivalência, onde cada classe representa um grupo de dados que o sistema processa de maneira semelhante. As classes de equivalência incluem tanto entradas válidas, que o sistema deve aceitar e processar, quanto entradas inválidas, que o sistema deve identificar e rejeitar adequadamente. Com esse método, é possível reduzir o número de testes necessários, focando apenas em casos representativos que têm maior probabilidade de revelar falhas, minimizando o esforço enquanto se maximiza a detecção de possíveis erros no sistema</p>
<br>


<table border="1">
  <tr> 
    <th  colspan =7>Classes de Equivalência</th>
  </tr>
  <tr>
    <th>Condição de Entrada</th>
    <th>Classes Válidas</th>
    <th>Classes Inválidas</th>
    <th>Classes Inválidas</th>
    <th>Classes Inválidas</th>
    <th>Classes Inválidas</th>
    <th>Classes Inválidas</th>
  </tr>
  <tr>
    <td>Nome</td>
    <td>1) somente letras (A-Z, a-z)</td>
    <td>2) contém dígitos (0-9)</td>
    <td>3) contém caracteres especiais (#, @, !, entre outros)</td>
    <td>4) campo vazio</td>
    <td>-</td>
    <td>-</td>
  </tr>
  <tr>
    <td>Email</td>
    <td>5) domínio padrão da ufam (nome@ufam.edu.br)</td>
    <td>6) fora do domínio padrão da ufam</td>
    <td>7) campo vazio</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
  </tr>
  <tr>
    <td>Siape</td>
    <td>8) 7 dígitos (0-9)</td>
    <td>9) contém letras (A-Z, a-z)</td>
    <td>10) contém caracteres especiais (#, @, !, entre outros)</td>
    <td>11) menos de 7 dígitos</td>
    <td>12) mais de 7 dígitos</td>
    <td>13) campo vazio</td>
  </tr>
  <tr>
    <td>Bloco</td>
    <td>14) 1 letra (A-F, a-f)</td>
    <td>15) letras fora do intervalo (G-Z, g-z)</td>
    <td>16) contém dígito (0-9)</td>
    <td>17) contém caractere especial (#, @, !)</td>
    <td>18) contém mais de 1 letra</td>
    <td>19) campo vazio</td>
  </tr>
  <tr>
    <td>Sala</td>
    <td>20) três dígitos (0-9)</td>
    <td>21) contém letras (A-Z, a-z)</td>
    <td>22) contém caracteres especiais (#, @, !, entre outros)</td>
    <td>23) contém mais de 3 dígitos</td>
    <td>24) contém menos de 3 dígitos</td>
    <td>25) campo vazio</td>
  </tr>
  <tr>
    <td>Descrição do Problema</td>
    <td>26) máximo 300 caracteres alfanuméricos (A-Z, a-z, 0-9)</td>
    <td>27) mais de 300 caracteres alfanuméricos</td>
    <td>28) campo vazio</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
  </tr>
</table>

<br>

<table border="1">
  <tr> 
    <th  colspan =7>Casos de Testes</th>
  </tr>
  <tr>
    <th>Nº Caso de Teste</th>
    <th>Classes de Equivalência</th>
    <th>Entradas</th>
    <th>Resultado Esperado</th>
  </tr>
  <tr>
    <td>1</td>
    <td>1, 5, 8, 14, 20, 26</td>
    <td>Entradas válidas</td>
    <td>Cadastro de solicitação de serviço realizado com sucesso</td>
  </tr>
  <tr>
    <td>2</td>
    <td>2, 5, 8, 14, 20, 26</td>
    <td>Nome inválido</td>
    <td>Falha no cadastro de solicitação de serviço, nome contém dígitos (0-9)</td>
  </tr>
  <tr>
    <td>3</td>
    <td>3, 5, 8, 14, 20, 26</td>
    <td>Nome inválido</td>
    <td>Falha no cadastro de solicitação de serviço, nome contém caracteres especiais (#, @, !, etc.)</td>
  </tr>
  <tr>
    <td>4</td>
    <td>4, 5, 8, 14, 20, 26</td>
    <td>Nome vazio</td>
    <td>Falha no cadastro de solicitação de serviço, campo de nome é obrigatório</td>
  </tr>
  <tr>
    <td>5</td>
    <td>1, 6, 8, 14, 20, 26</td>
    <td>Email inválido</td>
    <td>Falha no cadastro de solicitação de serviço, email fora do domínio padrão da ufam</td>
  </tr>
  <tr>
    <td>6</td>
    <td>1, 7, 8, 14, 20, 26</td>
    <td>Email vazio</td>
    <td>Falha no cadastro de solicitação de serviço, campo de email é obrigatório</td>
  </tr>
  <tr>
    <td>7</td>
    <td>1, 5, 9, 14, 20, 26</td>
    <td>Siape inválido</td>
    <td>Falha no cadastro de solicitação de serviço, siape contém letras (A-Z, a-z)</td>
  </tr>
  <tr>
    <td>8</td>
    <td>1, 5, 10, 14, 20, 26</td>
    <td>Siape inválido</td>
    <td>Falha no cadastro de solicitação de serviço, siape contém caracteres especiais (#, @, !, etc.)</td>
  </tr>
  <tr>
    <td>9</td>
    <td>1, 5, 11, 14, 20, 26</td>
    <td>Siape inválido</td>
    <td>Falha no cadastro de solicitação de serviço, siape contém menos de 7 dígitos</td>
  </tr>
  <tr>
    <td>10</td>
    <td>1, 5, 12, 14, 20, 26</td>
    <td>Siape inválido</td>
    <td>Falha no cadastro de solicitação de serviço, siape contém mais de 7 dígitos</td>
  </tr>
  <tr>
    <td>11</td>
    <td>1, 5, 13, 14, 20, 26</td>
    <td>Siape vazio</td>
    <td>Falha no cadastro de solicitação de serviço, campo de siape é obrigatório</td>
  </tr>
  <tr>
    <td>12</td>
    <td>1, 5, 8, 15, 20, 26</td>
    <td>Bloco inválido</td>
    <td>Falha no cadastro de solicitação de serviço, bloco com letra fora do intervalo (G-Z, g-z)</td>
  </tr>
  <tr>
    <td>13</td>
    <td>1, 5, 8, 16, 20, 26</td>
    <td>Bloco inválido</td>
    <td>Falha no cadastro de solicitação de serviço, bloco contém dígito (0-9)</td>
  </tr>
  <tr>
    <td>14</td>
    <td>1, 5, 8, 17, 20, 26</td>
    <td>Bloco inválido</td>
    <td>Falha no cadastro de solicitação de serviço, bloco contém caractere especial (#, @, !, etc.)</td>
  </tr>
  <tr>
    <td>15</td>
    <td>1, 5, 8, 18, 20, 26</td>
    <td>Bloco inválido</td>
    <td>Falha no cadastro de solicitação de serviço, bloco contém mais de uma letra</td>
  </tr>
  <tr>
    <td>16</td>
    <td>1, 5, 8, 19, 20, 26</td>
    <td>Bloco vazio</td>
    <td>Falha no cadastro de solicitação de serviço, campo bloco é obrigatório</td>
  </tr>
  <tr>
    <td>17</td>
    <td>1, 5, 8, 14, 21, 26</td>
    <td>Sala inválido</td>
    <td>Falha no cadastro de solicitação de serviço, sala contém letras (A-Z, a-z)</td>
  </tr>
  <tr>
    <td>18</td>
    <td>1, 5, 8, 14, 22, 26</td>
    <td>Sala inválido</td>
    <td>Falha no cadastro de solicitação de serviço, sala contém caracteres especiais (#, @, !, etc.)</td>
  </tr>
  <tr>
    <td>19</td>
    <td>1, 5, 8, 14, 23, 26</td>
    <td>Sala inválido</td>
    <td>Falha no cadastro de solicitação de serviço, sala contém mais de 3 dígitos</td>
  </tr>
  <tr>
    <td>20</td>
    <td>1, 5, 8, 14, 24, 26</td>
    <td>Sala inválido</td>
    <td>Falha no cadastro de solicitação de serviço, sala contém menos de 3 dígitos</td>
  </tr>
  <tr>
    <td>21</td>
    <td>1, 5, 8, 14, 25, 26</td>
    <td>Sala vazio</td>
    <td>Falha no cadastro de solicitação de serviço, campo sala é obrigatório</td>
  </tr>
  <tr>
    <td>22</td>
    <td>1, 5, 8, 14, 20, 27</td>
    <td>Descrição do Problema inválido</td>
    <td>Falha no cadastro de solicitação de serviço, descrição do problema contém mais de 300 caracteres</td>
  </tr>
  <tr>
    <td>23</td>
    <td>1, 5, 8, 14, 20, 28</td>
    <td>Descrição do Problema vazio</td>
    <td>Falha no cadastro de solicitação de serviço, campo descrição do problema é obrigatório</td>
  </tr>
</table>

