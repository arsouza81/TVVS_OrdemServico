# Plano de Testes - Sistema de Ordem de Serviço

- **Nome do Projeto:** Sistema Ordem de Serviço
- **Versão do Plano de Teste:** 1.0
- **Data de Criação:** 04/11/2024
- **Data de Revisão:** -
- **Nome do Gerente de Testes:** Kassia Ramos Oliveira
- **Equipe de Testes:** Alicia Caldeira da Silva, Anderson Rodrigues de Souza, Diandre Pires Bruce e Rennan de Souza Alves

## 1. Escopo e Objetivo

<p align=justify>O sistema de Ordem de Serviço foi desenvolvido para otimizar e simplificar o processo de solicitação de serviços de TI entre os servidores do Instituto Federal de Ciências Exatas e Tecnologia (ICET) e a equipe de suporte da Gerência de TI. Seu objetivo principal é criar um canal único e organizado para que os usuários possam registrar suas solicitações de maneira prática e centralizada, facilitando a gestão e o acompanhamento dessas demandas. Por meio do sistema, os usuários conseguem descrever o problema ou serviço necessário, especificar sua localização e encaminhar a solicitação diretamente para o setor responsável, tudo em uma interface de fácil acesso.</p>

<p align=justify>Além disso, o sistema de Ordem de Serviço oferece um ambiente seguro para o registro e armazenamento das informações, garantindo que todos os dados das solicitações estejam protegidos e possam ser acessados pela equipe de TI de forma estruturada. A Gerência de TI é notificada a cada nova solicitação, o que permite uma resposta ágil e direcionada às demandas. O sistema também inclui funcionalidades que permitem ao usuário acompanhar o status de suas solicitações em tempo real, desde o registro inicial até a conclusão do serviço, com atualizações automáticas e notificações sobre o andamento. Dessa forma, o sistema busca não apenas facilitar a comunicação entre os servidores e a equipe de TI, mas também aumentar a eficiência do processo de atendimento, proporcionando maior transparência e controle para ambos os lados.</p>

## 2. Características do produto a serem testadas

<p align=justify>O sistema Ordem de Serviço, é um sistema com funcionalidades básicas e objetivas, nesta parte do documento, vamos apresentar as funcionalidades classificadas para os testes, a equipe de testes desenvolveu os casos de teste na funcionalidades que julgaram mais críticas do sistema e estão descritas abaixo, juntamento com seus subcasos de testes.</p>

- Cadastro de Solicitações de Serviços
  - Validação do campo Nome
  - Validação do campo Email
  - Validação do campo Siape
  - Validação do campo Bloco
  - Validação do campo Sala
  - Validação do campo Descrição do Problema

- Login da Gerência
  - Validação do Campo Email.
  - Validação do Campo senha.


- Busca de Protocolo no sistema
  - Validação do código de protocolo para busca.

## 3. Abordagem a ser uitilizada

<p align=justify>A abordagem de teste do sistema de Ordem de Serviço define técnicas, métodos e ferramentas específicas para garantir que todas as funcionalidades e fluxos do sistema sejam validados de maneira abrangente. A abordagem inclui testes funcionais, assegurando que o sistema atenda às necessidades dos usuários do Instituto Federal de Ciências Exatas e Tecnologia (ICET).</p>

<table>
  <tr>
    <th>Item</th>
    <th colspan=4>Descrição</th>
  </tr>
  <tr>
    <td><b>Objetivo</b></td>
    <td colspan=4 aling=justify>Verificar se o processo de cadastro de solicitação de serviços atende às especificações dos requisitos, validando os campos nome, email, siape, bloco, sala e descrição do problema do formulário de cadastro de ordem de serviço.</td>
  </tr>
  <tr>
    <td><b>Técnica</b></td>
    <td colspan=2>( ) Manual</td>
    <td colspan=2>(X) Automática</td>
  </tr>
  <tr>
    <td><b>Estágio do Teste</b></td>
    <td>(X) Unidade</td>
    <td>( ) Integração</td>
    <td>( ) Sistema</td>
    <td>( ) Aceitação</td>
  </tr>
  <tr>
    <td><b>Abordagem do Teste</b></td>
    <td colspan=2>( ) Caixa Branca</td>
    <td colspan=2>(X) Caixa Preta</td>
  </tr>
  <tr>
    <td><b>Responsáveis</b></td>
    <td colspan=4>Equipe de Testes</td>
  </tr>
</table>

**Testes Funcionais:** Testar todo o fluxo do processo para o cadastro de solicitações de serviços, validando os campos nome, email, siape, bloco, sala e descrição do problema do formulário de cadastro de ordem de serviço. <br>
**Ferramentas utilizadas:** XUnit (Teste de Unidade).

## 4. Itens a serem testados

<p align = justify>Serão testados todos os campos do formulário de cadastro de solicitações de serviços, com o objetivo de verificar o fluxo para o processo de cadastro das solicitações a partir da:</p>

- Validação do campo Nome.
- Validação do campo Email.
- Validação do campo Siape.
- Validação do campo Bloco.
- Validação do campo Sala.
- Validação do campo Descrição do Problema.

## 5. Cronograma para o Teste

<p align = justify>O cronograma do sistema de Ordem de Serviço define os prazos estimados para a execução de cada fase essencial do plano de testes, garantindo que todas as atividades sejam organizadas e realizadas dentro de um período adequado. Esse cronograma detalha o tempo necessário para preparar o ambiente de testes, definir os casos e cenários a serem testados, realizar os testes funcionais e revisar os resultados de cada etapa.</p>
<p align = justify>O planejamento temporal é fundamental para assegurar que cada fase do teste contribua para a identificação de possíveis problemas antes do lançamento do sistema. Com isso, o cronograma facilita o acompanhamento do progresso e permite ajustes quando necessário, garantindo que o sistema atenda a todos os requisitos de qualidade no prazo estabelecido. Além disso, ele ajuda a coordenar as equipes envolvidas, organizando as tarefas de modo que os recursos estejam disponíveis e as etapas possam ser realizadas sequencialmente ou em paralelo, conforme o plano do projeto. Dessa forma, o cronograma contribui diretamente para que o sistema de Ordem de Serviço seja entregue com eficiência, qualidade e dentro do período esperado.</p>

- **Semana 1:** Revisão do plano de testes e preparação do ambiente.
- **Semana 2-3:** Execução dos testes funcionais na funcionalidade de cadastro de solicitações de serviços.
- **Semana 4:** Avaliação final, relatório de bugs e liberação para produção.

## 6. Pessoal responsável pelas diferentes atividades de teste

<p align = justify>A lista dos testadores identifica detalhadamente os responsáveis por cada atividade ou etapa específica do processo de testes do sistema de Ordem de Serviço. Esse documento é fundamental para organizar e distribuir as tarefas entre a equipe de testes, garantindo que cada membro esteja ciente das suas atribuições e responsabilidades. A lista especifica quem estará encarregado de conduzir os testes funcionais, bem como os responsáveis pelo planejamento dos cenários de teste, execução dos scripts de teste automatizados e análise dos resultados obtidos.</p>
<p align = justify>Além de definir a atuação individual, a lista facilita a coordenação do trabalho em equipe, assegurando que as atividades de teste ocorram de forma integrada e eficiente. Ela também possibilita uma visão clara de quem procurar em caso de dúvidas ou problemas em cada fase do processo de testes, promovendo a comunicação entre os membros e o alinhamento dos esforços. Dessa maneira, a lista dos testadores contribui para que o processo de validação do sistema ocorra de maneira organizada e dentro dos prazos estabelecidos, assegurando que todas as funcionalidades do sistema de Ordem de Serviço sejam testadas de forma completa e minuciosa.</p>

- **Responsáveis por Testes Funcionais:** Anderson Rodrigues de Souza e Alicia Caldeira da Silva
- **Responsável por Automação de Testes:** Rennan de Souza Alves
- **Gerente de Testes:** Kassia Ramos Oliveira
- **Analista de Qualidade:** Diandre Pires Bruce

## 7. Os riscos associados aos testes

<p align = justify>Os riscos associados ao processo de testes incluem possíveis problemas que podem afetar a execução das atividades de validação ou o sucesso do sistema. Identificar e planejar a mitigação desses riscos é essencial para manter o cronograma de testes e assegurar a entrega de um produto de alta qualidade.</p>

**Riscos Específicos para o Sistema de Ordem de Serviço:**

- **Dependência de Integração com Serviços Internos:** Caso o serviço de envio de acesso ao banco de dados não esteja plenamente operacional no ambiente de testes, a execução pode ser comprometida, resultando em atrasos e dificuldade para simular adequadamente as funcionalidades.
- **Recursos Limitados na Equipe de Testes:** Se o número de testadores for insuficiente para cobrir todos os casos e cenários dentro do prazo estipulado, isso poderá resultar em falhas de cobertura dos testes. Isso afetaria a identificação de possíveis problemas no sistema, especialmente em casos de uso menos frequentes mas críticos para a operação.
- **Ambiente de Teste Não Alinhado com o Ambiente Real:** Caso o ambiente de testes não simule com precisão o ambiente de produção, há o risco de que certos problemas não sejam detectados durante os testes, resultando em falhas quando o sistema estiver em uso.

<p align = justify>Esses riscos devem ser continuamente monitorados e, sempre que possível, medidas preventivas e planos de contingência devem ser implementados para reduzir o impacto no processo de testes e garantir a entrega de um sistema de Ordem de Serviço confiável e eficiente.</p>

<br>

# Especificação dos Casos de Teste

## 1. Caracterização do Caso de Teste

<p align = justify>Cada caso de teste representa uma situação particular ou uma funcionalidade específica do Sistema de Ordem de Serviço que deve ser analisada detalhadamente. Através desses testes, verifica-se o comportamento do sistema em diferentes cenários, garantindo que ele esteja executando corretamente as tarefas para as quais foi projetado. Essa abordagem é essencial para identificar possíveis erros ou falhas, permitindo que sejam feitos ajustes antes que o sistema seja utilizado em um ambiente de produção. Assim, os casos de teste são uma ferramenta importante para assegurar que o sistema atende aos requisitos definidos e funciona de acordo com as expectativas dos usuários.</p>

<table border="1">
  <tr>
    <th>Identificador</th>
    <td>CT-01</td>
  </tr>
  <tr>
    <th>Caso de teste</th>
    <td>Finalizar o cadastro de solicitação de serviço</td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>Verificar se os campos do cadastro de solicitação de serviço foram preenchidos corretamente.</td>
  </tr>
  <tr>
    <th>Entradas</th>
    <td>. Nome: "Leilane Cardoso".<br>. Email: "leilCardoso@ufam.edu.br".<br>. Siape: "1234567".<br>. Bloco: "C".<br>. Sala: "301".<br>. Descrição do Problema: "Computador reiniciando automaticamente"</td>
  </tr>
  <tr>
    <th>Resultados Esperados</th>
    <td>. Se os campos estiverem preenchidos corretamente, o cadastro da solicitação é realizado com sucesso.<br>. Se os campos não estiverem preenchidos corretamente, uma mensagem de erro deve ser exibida informando o campo e o erro a serem corrigidos.</td>
  </tr>
  <tr>
    <th>Critérios para Aprovação/Rejeição</th>
    <td>. Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.</td>
  </tr>
  <tr>
    <th>Recursos para o Caso de Teste</th>
    <td>. Ambiente de Teste: Navegador e banco de dados do sistema. . Ferramentas: XUnit</td>
  </tr>
  <tr>
    <th>Restrições de Uso</th>
    <td>. Todos os campos devem ser preenchidos corretamente.</td>
  </tr>
  <tr>
    <th>Dependências</th>
    <td>Não se aplica</td>
  </tr>
  <tr>
    <th>Observações Adicionais</th>
    <td>. Realizar testes com diversos dados para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
  </tr>
</table>

<br>

<table border="1">
  <tr>
    <th>Identificador</th>
    <td>CT-02</td>
  </tr>
  <tr>
    <th>Caso de teste</th>
    <td>Validar o campo nome para finalizar o cadastro de solicitação de serviço</td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>Verificar se o nome do solicitante é informado corretamente, sendo composto apenas por letras</td>
  </tr>
  <tr>
    <th>Entradas</th>
    <td>. Nome: "Leil4ne Cardoso"</td>
  </tr>
  <tr>
    <th>Resultados Esperados</th>
    <td>. Se o nome for composto apenas por letras, o cadastro da solicitação é realizado com sucesso.<br>. Se o nome não for composto apenas por letras, uma mensagem de erro deve ser exibida informando o erro.</td>
  </tr>
  <tr>
    <th>Critérios para Aprovação/Rejeição</th>
    <td>. Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.</td>
  </tr>
  <tr>
    <th>Recursos para o Caso de Teste</th>
    <td>. Ambiente de Teste: Navegador e banco de dados do sistema.<br>. Ferramentas: XUnit</td>
  </tr>
  <tr>
    <th>Restrições de Uso</th>
    <td>. O nome é um campo obrigatório e deve conter apenas letras, não pode ter dígitos, caracteres especiais</td>
  </tr>
  <tr>
    <th>Dependências</th>
    <td>Não se aplica</td>
  </tr>
  <tr>
    <th>Observações Adicionais</th>
    <td>. Realizar testes com diferentes sequências de nomes para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
  </tr>
</table>

<br>

<table border="1">
  <tr>
    <th>Identificador</th>
    <td>CT-03</td>
  </tr>
  <tr>
    <th>Caso de teste</th>
    <td>Validar o campo nome para finalizar o cadastro de solicitação de serviço</td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>Verificar se o nome do solicitante é informado corretamente, sendo composto apenas por letras</td>
  </tr>
  <tr>
    <th>Entradas</th>
    <td>. Nome: "Leil#ne Cardoso"</td>
  </tr>
  <tr>
    <th>Resultados Esperados</th>
    <td>. Se o nome for composto apenas por letras, o cadastro da solicitação é realizado com sucesso.<br>. Se o nome não for composto apenas por letras, uma mensagem de erro deve ser exibida informando o erro.</td>
  </tr>
  <tr>
    <th>Critérios para Aprovação/Rejeição</th>
    <td>. Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.</td>
  </tr>
  <tr>
    <th>Recursos para o Caso de Teste</th>
    <td>. Ambiente de Teste: Navegador e banco de dados do sistema.<br>. Ferramentas: XUnit</td>
  </tr>
  <tr>
    <th>Restrições de Uso</th>
    <td>. O nome é um campo obrigatório e deve conter apenas letras, não pode ter dígitos, caracteres especiais</td>
  </tr>
  <tr>
    <th>Dependências</th>
    <td>Não se aplica</td>
  </tr>
  <tr>
    <th>Observações Adicionais</th>
    <td>. Realizar testes com diferentes sequências de nomes para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
  </tr>
</table>

<br>

<table border="1">
  <tr>
    <th>Identificador</th>
    <td>CT-04</td>
  </tr>
  <tr>
    <th>Caso de teste</th>
    <td>Validar o campo nome para finalizar o cadastro de solicitação de serviço</td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>Verificar se o nome do solicitante é informado corretamente, sendo composto apenas por letras</td>
  </tr>
  <tr>
    <th>Entradas</th>
    <td>Nome: "    "</td>
  </tr>
  <tr>
    <th>Resultados Esperados</th>
    <td>. Se o nome for composto apenas por letras, o cadastro da solicitação é realizado com sucesso.<br>. Se o nome não for composto apenas por letras, uma mensagem de erro deve ser exibida informando o erro.</td>
  </tr>
  <tr>
    <th>Critérios para Aprovação/Rejeição</th>
    <td>. Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.</td>
  </tr>
  <tr>
    <th>Recursos para o Caso de Teste</th>
    <td>. Ambiente de Teste: Navegador e banco de dados do sistema.<br>. Ferramentas: XUnit</td>
  </tr>
  <tr>
    <th>Restrições de Uso</th>
    <td>O nome é um campo obrigatório e deve conter apenas letras, não podendo ter dígitos e caracteres especiais</td>
  </tr>
  <tr>
    <th>Dependências</th>
    <td>Não se aplica</td>
  </tr>
  <tr>
    <th>Observações Adicionais</th>
    <td>. Realizar testes com diferentes sequências de nomes para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
  </tr>
</table>

<br>

<table border="1">
  <tr>
    <th>Identificador</th>
    <td>CT-05</td>
  </tr>
  <tr>
    <th>Caso de teste</th>
    <td>Validar o campo email para finalizar o cadastro de solicitação de serviço</td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>Verificar se o email do solicitante é informado corretamente, seguindo o domínio padrão da UFAM (nome@ufam.edu.br)</td>
  </tr>
  <tr>
    <th>Entradas</th>
    <td>Email: "leilCardoso@gmail.com"</td>
  </tr>
  <tr>
    <th>Resultados Esperados</th>
    <td>. Se o email seguir o domínio padrão da UFAM (nome@ufam.edu.br), o cadastro da solicitação é realizado com sucesso.<br>. Se o email não seguir o domínio padrão da UFAM (nome@ufam.edu.br), uma mensagem de erro deve ser exibida informando o erro.</td>
  </tr>
  <tr>
    <th>Critérios para Aprovação/Rejeição</th>
    <td>. Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.</td>
  </tr>
  <tr>
    <th>Recursos para o Caso de Teste</th>
    <td>Ambiente de Teste: Navegador e banco de dados do sistema.<br>. Ferramentas: XUnit</td>
  </tr>
  <tr>
    <th>Restrições de Uso</th>
    <td>O email é um campo obrigatório e deve seguir o domínio padrão da UFAM (nome@ufam.edu.br)</td>
  </tr>
  <tr>
    <th>Dependências</th>
    <td>O caso de teste "Validar o campo email para finalizar o cadastro de solicitação de serviço" depende do caso de teste "Validar o campo nome para finalizar o cadastro de solicitação de serviço".</td>
  </tr>
  <tr>
    <th>Observações Adicionais</th>
    <td>. Realizar testes com diferentes domínios de emails para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
  </tr>
</table>

<br>

<table border="1">
  <tr>
    <th>Identificador</th>
    <td>CT-06</td>
  </tr>
  <tr>
    <th>Caso de teste</th>
    <td>Validar o campo email para finalizar o cadastro de solicitação de serviço</td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>Verificar se o email do solicitante é informado corretamente, seguindo o domínio padrão da UFAM (nome@ufam.edu.br)</td>
  </tr>
  <tr>
    <th>Entradas</th>
    <td>Email: " "</td>
  </tr>
  <tr>
    <th>Resultados Esperados</th>
    <td>. Se o email seguir o domínio padrão da UFAM (nome@ufam.edu.br), o cadastro da solicitação é realizado com sucesso.<br>. Se o email não seguir o domínio padrão da UFAM (nome@ufam.edu.br), uma mensagem de erro deve ser exibida informando o erro.</td>
  </tr>
  <tr>
    <th>Critérios para Aprovação/Rejeição</th>
    <td>. Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.</td>
  </tr>
  <tr>
    <th>Recursos para o Caso de Teste</th>
    <td>Ambiente de Teste: Navegador e banco de dados do sistema. Ferramentas: XUnit</td>
  </tr>
  <tr>
    <th>Restrições de Uso</th>
    <td>O email é um campo obrigatório e deve seguir o domínio padrão da UFAM (nome@ufam.edu.br)</td>
  </tr>
  <tr>
    <th>Dependências</th>
    <td>O caso de teste "Validar o campo email para finalizar o cadastro de solicitação de serviço" depende do caso de teste "Validar o campo nome para finalizar o cadastro de solicitação de serviço".</td>
  </tr>
  <tr>
    <th>Observações Adicionais</th>
    <td>. Realizar testes com diferentes domínios de emails para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
  </tr>
</table>

<br>

<table border="1">
    <tr>
        <th>Identificador</th>
        <td>CT-07</td>
    </tr>
    <tr>
        <th>Caso de teste</strong></th>
        <td>Validar o campo siape para finalizar o cadastro de solicitação de serviço</td>
    </tr>
    <tr>
        <th>Descrição</th>
        <td>Verificar se o siape do solicitante é informado corretamente, sendo composto por 7 dígitos (0-9)</td>
    </tr>
    <tr>
        <th>Entradas</th>
        <td>Siape: "123d567"</td>
    </tr>
    <tr>
        <th>Resultados Esperados</th>
        <td>
            . Se o siape for composto, exatamente, por 7 dígitos (0-9), o cadastro da solicitação é realizado com sucesso.<br>. Se o siape não for composto por apenas dígitos, ou for composto por mais de 7 dígitos, ou for composto por menos de 7 dígitos, uma mensagem de erro deve ser exibida informando o erro.
        </td>
    </tr>
    <tr>
        <th>Critérios para Aprovação/Rejeição</th>
        <td>
            . Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.
        </td>
    </tr>
    <tr>
        <th>Recursos para o Caso de Teste</th>
        <td>
            . Ambiente de Teste: Navegador e banco de dados do sistema. <br>. Ferramentas: XUnit
        </td>
    </tr>
    <tr>
        <td><strong>Restrições de Uso</strong></td>
        <td>O siape é um campo obrigatório e deve ser composto por 7 dígitos (0-9).</td>
    </tr>
    <tr>
        <th>Dependências</th>
        <td>O caso de teste "Validar o campo siape para finalizar o cadastro de solicitação de serviço" depende do caso de teste "Validar o campo email para finalizar o cadastro de solicitação de serviço".</td>
    </tr>
    <tr>
        <th>Observações Adicionais</th>
        <td>. Realizar testes com diferentes sequências de dígitos, letras e caracteres especiais para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
    </tr>
</table>

<br>

<table border="1">
    <tr>
        <th>Identificador</th>
        <td>CT-08</td>
    </tr>
    <tr>
        <th>Caso de teste</th>
        <td>Validar o campo siape para finalizar o cadastro de solicitação de serviço</td>
    </tr>
    <tr>
        <th>Descrição</th>
        <td>Verificar se o siape do solicitante é informado corretamente, sendo composto por 7 dígitos (0-9)</td>
    </tr>
    <tr>
        <th>Entradas</th>
        <td>Siape: "!234567"</td>
    </tr>
    <tr>
        <th>Resultados Esperados</th>
        <td>
            . Se o siape for composto, exatamente, por 7 dígitos (0-9), o cadastro da solicitação é realizado com sucesso.<br>. Se o siape não for composto por apenas dígitos, ou for composto por mais de 7 dígitos, ou for composto por menos de 7 dígitos, uma mensagem de erro deve ser exibida informando o erro.
        </td>
    </tr>
    <tr>
        <th>Critérios para Aprovação/Rejeição</th>
        <td>
            . Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.
        </td>
    </tr>
    <tr>
        <th>Recursos para o Caso de Teste</th>
        <td>
            . Ambiente de Teste: Navegador e banco de dados do sistema.<br>. Ferramentas: XUnit
        </td>
    </tr>
    <tr>
       <th>Restrições de Uso</th>
        <td>O siape é um campo obrigatório e deve ser composto por 7 dígitos (0-9).</td>
    </tr>
    <tr>
        <th>Dependências</th>
        <td>O caso de teste "Validar o campo siape para finalizar o cadastro de solicitação de serviço" depende do caso de teste "Validar o campo email para finalizar o cadastro de solicitação de serviço".</td>
    </tr>
    <tr>
        <th>Observações Adicionais</th>
        <td>. Realizar testes com diferentes sequências de dígitos, letras e caracteres especiais para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
    </tr>
</table>

<br>

<table border="1">
    <tr>
        <th>Identificador</th>
        <td>CT-09</td>
    </tr>
    <tr>
        <th>Caso de teste</th>
        <td>Validar o campo siape para finalizar o cadastro de solicitação de serviço</td>
    </tr>
    <tr>
        <th>Descrição</th>
        <td>Verificar se o siape do solicitante é informado corretamente, sendo composto por 7 dígitos (0-9)</td>
    </tr>
    <tr>
        <th>Entradas</th>
        <td>Siape: "123456"</td>
    </tr>
    <tr>
        <th>Resultados Esperados</th>
        <td>
            . Se o siape for composto, exatamente, por 7 dígitos (0-9), o cadastro da solicitação é realizado com sucesso.<br>. Se o siape não for composto por apenas dígitos, ou for composto por mais de 7 dígitos, ou for composto por menos de 7 dígitos, uma mensagem de erro deve ser exibida informando o erro.
        </td>
    </tr>
    <tr>
        <th>Critérios para Aprovação/Rejeição</th>
        <td>
            . Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.
        </td>
    </tr>
    <tr>
        <th>Recursos para o Caso de Teste</th>
        <td>
            . Ambiente de Teste: Navegador e banco de dados do sistema.<br>. Ferramentas: XUnit.
        </td>
    </tr>
    <tr>
        <th>Restrições de Uso</th>
        <td>O siape é um campo obrigatório e deve ser composto por 7 dígitos (0-9).</td>
    </tr>
    <tr>
        <th>Dependências</th>
        <td>O caso de teste "Validar o campo siape para finalizar o cadastro de solicitação de serviço" depende do caso de teste "Validar o campo email para finalizar o cadastro de solicitação de serviço".</td>
    </tr>
    <tr>
        <th>Observações Adicionais</th>
        <td>. Realizar testes com diferentes sequências de dígitos, letras e caracteres especiais para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
    </tr>
</table>

<br>

<table border="1">
    <tr>
        <th>Identificador</th>
        <td>CT-10</td>
    </tr>
    <tr>
        <th>Caso de teste</th>
        <td>Validar o campo siape para finalizar o cadastro de solicitação de serviço</td>
    </tr>
    <tr>
        <th>Descrição</th>
        <td>Verificar se o siape do solicitante é informado corretamente, sendo composto por 7 dígitos (0-9)</td>
    </tr>
    <tr>
        <th>Entradas</th>
        <td>Siape: "12345678"</td>
    </tr>
    <tr>
        <th>Resultados Esperados</th>
        <td>
            . Se o siape for composto, exatamente, por 7 dígitos (0-9), o cadastro da solicitação é realizado com sucesso.<br>. Se o siape não for composto por apenas dígitos, ou for composto por mais de 7 dígitos, ou for composto por menos de 7 dígitos, uma mensagem de erro deve ser exibida informando o erro.
        </td>
    </tr>
    <tr>
        <th>Critérios para Aprovação/Rejeição</th>
        <td>
            . Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.
        </td>
    </tr>
    <tr>
        <th>Recursos para o Caso de Teste</th>
        <td>
            . Ambiente de Teste: Navegador e banco de dados do sistema.<br>. Ferramentas: XUnit.
        </td>
    </tr>
    <tr>
        <th>Restrições de Uso</th>
        <td>O siape é um campo obrigatório e deve ser composto por 7 dígitos (0-9).</td>
    </tr>
    <tr>
        <th>Dependências</th>
        <td>O caso de teste "Validar o campo siape para finalizar o cadastro de solicitação de serviço" depende do caso de teste "Validar o campo email para finalizar o cadastro de solicitação de serviço".</td>
    </tr>
    <tr>
        <th>Observações Adicionais</th>
        <td>. Realizar testes com diferentes sequências de dígitos, letras e caracteres especiais para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
    </tr>
</table>

<br>

<table border="1">
    <tr>
        <th>Identificador</th>
        <td>CT-11</td>
    </tr>
    <tr>
        <th>Caso de teste</th>
        <td>Validar o campo siape para finalizar o cadastro de solicitação de serviço</td>
    </tr>
    <tr>
        <th>Descrição</th>
        <td>Verificar se o siape do solicitante é informado corretamente, sendo composto por 7 dígitos (0-9)</td>
    </tr>
    <tr>
        <th>Entradas</th>
        <td>Siape: "  "</td>
    </tr>
    <tr>
        <th>Resultados Esperados</th>
        <td>
            . Se o siape for composto, exatamente, por 7 dígitos (0-9), o cadastro da solicitação é realizado com sucesso.<br>. Se o siape não for composto por apenas dígitos, ou for composto por mais de 7 dígitos, ou for composto por menos de 7 dígitos, uma mensagem de erro deve ser exibida informando o erro.
        </td>
    </tr>
    <tr>
        <th>Critérios para Aprovação/Rejeição</th>
        <td>
            . Aprovação: O cadastro da solicitação de serviço é realizado com sucesso.<br>. Rejeição: O cadastro da solicitação de serviço não é realizado e o sistema exibe uma mensagem informando o erro.
        </td>
    </tr>
    <tr>
        <th>Recursos para o Caso de Teste</th>
        <td>
            . Ambiente de Teste: Navegador e banco de dados do sistema.<br>. Ferramentas: XUnit
        </td>
    </tr>
    <tr>
        <th>Restrições de Uso</th>
        <td>O siape é um campo obrigatório e deve ser composto por 7 dígitos (0-9).</td>
    </tr>
    <tr>
        <th>Dependências</th>
        <td>O caso de teste "Validar o campo siape para finalizar o cadastro de solicitação de serviço" depende do caso de teste "Validar o campo email para finalizar o cadastro de solicitação de serviço".</td>
    </tr>
    <tr>
        <th>Observações Adicionais</th>
        <td>. Realizar testes com diferentes sequências de dígitos, letras e caracteres especiais para garantir a eficácia e a cobertura dos testes.<br>. Documentar quaisquer anomalias ou comportamentos inesperados.</td>
    </tr>
</table>

<br>


## 2. Especificação de Entradas, Resultados Esperados e Casos de Testes

<p align = justify>Esta seção abordará em detalhes as diferentes entradas que o sistema deverá processar, especificando os resultados esperados para cada uma dessas entradas ao serem analisadas. O objetivo é descrever como o sistema deve responder em cada situação prevista, garantindo que o comportamento seja conforme esperado. Para alcançar essa validação de forma eficiente, será aplicada a técnica de particionamento por classes de equivalência.</p>

<p align = justify> A técnica de particionamento por classes de equivalência, amplamente utilizada em testes de software, consiste em dividir o conjunto de possíveis entradas em classes de equivalência, onde cada classe representa um grupo de dados que o sistema processa de maneira semelhante. As classes de equivalência incluem tanto entradas válidas, que o sistema deve aceitar e processar, quanto entradas inválidas, que o sistema deve identificar e rejeitar adequadamente. Com esse método, é possível reduzir o número de testes necessários, focando apenas em casos representativos que têm maior probabilidade de revelar falhas, minimizando o esforço enquanto se maximiza a detecção de possíveis erros no sistema</p>
<br>

## 3. Abordagem a ser utilizada


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

