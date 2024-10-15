# Validação de Sistema

## Avaliadora 1

## Objetivos e Escopo da Avaliação

O objetivo desta avaliação é realizar uma inspeção heurística do sistema, analisando suas interfaces e fluxos de interação, identificando problemas de usabilidade e violações de heurísticas de Nielsen. O escopo da avaliação abrange a verificação de sete telas do sistema, com foco em usabilidade e prevenção de erros.

## Método Utilizado

Para a validação, foi adotada a **inspeção heurística** baseada nas **10 heurísticas de usabilidade de Nielsen**. Os avaliadores inspecionaram o sistema de maneira independente, focando em problemas de usabilidade e propondo soluções para melhorar a interface e a experiência do usuário.

### Conjunto de Heurísticas Utilizado:
1. **H1. Visibilidade do status do sistema**
2. **H2. Compatibilidade entre o sistema e o mundo real**
3. **H3. Controle e liberdade do usuário**
4. **H5. Prevenção de erros**
5. **H6. Reconhecer ao invés de lembrar**
6. **H7. Flexibilidade e eficiência de uso**
7. **H8. Estética e design minimalista**
8. **H9. Ajuda a reconhecer, diagnosticar e corrigir erros**
9. **H10. Ajuda e documentação**

## Perfil e Quantidade dos Avaliadores

As avaliadoras as avaliadoras possuem bom entendimento de interfaces web. No total, 2 (duas) avaliadoras participaram do processo de inspeção.

### Avaliadora 1: Técnica em Desenvolvimento de Sistemas

**Nome:** Alicia Caldeira da Silva

**Formação:** Técnica em Desenvolvimento de Sistemas

**Curso:** Engenharia de Software

**Experiência:** 
- Participou de avaliações de usabilidade em projetos anteriores, contribuindo na identificação de problemas de interface e inconsistências na interação do usuário.

### Avaliadora 2: Técnica em Informática

**Nome:** Diandre Pires Bruce

**Formação:** Técnica em Informática

**Curso:** Engenharia de Software

**Experiência:** 
- Já realizou avaliações de usabilidade em projetos anteriores, contribuindo na identificação de problemas de interface e inconsistências na interação do usuário.

## Processo de Inspeção

O processo foi dividido nas seguintes fases:

1. **Detecção de Defeitos**: Os avaliadores inspecionaram as telas do sistema, buscando defeitos e violações das heurísticas de usabilidade.
2. **Coleção de Defeitos**: Os defeitos encontrados foram coletados e organizados para avaliação.
3. **Discriminação de Defeitos**: Os defeitos foram analisados e categorizados de acordo com o grau de severidade e a heurística violada.

## Lista de Problemas de Usabilidade Encontrados

### Tela 1:
- **H1. Visibilidade do status do sistema** (Severidade: 4)  
  - **Ponto positivo**: Há um botão "Buscar" e campos de preenchimento claros.
  - **Sugestão**: Incluir feedback visual ou mensagem quando uma ordem de serviço for inexistente.

- **H2. Compatibilidade entre o sistema e o mundo real** (Severidade: 1)  
  - **Ponto positivo**: Termos como "Nome", "Email", e "Descrição do Problema" são familiares aos usuários.
  - **Sugestão**: Incluir uma explicação para o termo "Siape", que pode ser desconhecido para alguns usuários.

- **H3. Controle e liberdade do usuário** (Severidade: 2)  
  - **Análise**: Não há opção de editar ou revisar informações antes de enviar.
  - **Sugestão**: Permitir a revisão de dados ou a inclusão de um botão "Cancelar" para evitar submissões acidentais.

- **H5. Prevenção de erros** (Severidade: 3)  
  - **Análise**: Não há validações nos campos obrigatórios.
  - **Sugestão**: Implementar validação nos campos, como endereço de e-mail válido.

- **H9. Ajuda os usuários a reconhecer, diagnosticar e corrigir erros** (Severidade: 4)  
  - **Análise**: Não há feedback para erros no envio do formulário.
  - **Sugestão**: Incluir mensagens de erro específicas, como "Campo obrigatório" ou "Insira um e-mail válido".

- **H10. Ajuda e documentação** (Severidade: 2)  
  - **Análise**: Não há ajuda visível.
  - **Sugestão**: Incluir um botão para acessar uma seção de ajuda ou FAQ.

---

### Tela 2:
- **H3. Controle e liberdade do usuário** (Severidade: 3)  
  - **Análise**: Há um link "voltar", mas a opção de visualizar senhas enquanto digita melhoraria a experiência.

- **H5. Ajudar os usuários a reconhecer, diagnosticar e corrigir erros** (Severidade: 3)  
  - **Análise**: Não há validação em tempo real para campos como e-mail ou senha.
  - **Sugestão**: Implementar validações em tempo real com mensagens claras, como "E-mail inválido".

- **H8. Estética e design minimalista** (Severidade: 2)  
  - **Ponto positivo**: Design limpo e minimalista.
  - **Sugestão**: O centro da tela está vazio, poderia haver uma breve explicação ou imagem para preencher o espaço.

- **H10. Ajuda e documentação** (Severidade: 2)  
  - **Análise**: Não há links de ajuda visíveis.
  - **Sugestão**: Incluir um link para suporte técnico.

---

### Tela 3:
- **H3. Controle e liberdade do usuário** (Severidade: 3)  
  - **Análise**: Não há opção de retornar à página anterior.
  - **Sugestão**: Incluir a opção de voltar.

- **H9. Ajuda os usuários a reconhecer, diagnosticar e corrigir erros** (Severidade: 4)  
  - **Análise**: Não há mensagens de erro para solicitações não encontradas.
  - **Sugestão**: Incluir uma mensagem clara quando uma solicitação não for encontrada.

---

### Tela 4:
- **H7. Flexibilidade e eficiência de uso** (Severidade: 2)  
  - **Análise**: O calendário é útil, mas seria interessante permitir a seleção de um intervalo de datas.
  - **Sugestão**: Implementar filtros adicionais ou intervalos de datas.

- **H9. Ajuda os usuários a reconhecer, diagnosticar e corrigir erros** (Severidade: 3)  
  - **Análise**: Não há feedback para erros de pesquisa.
  - **Sugestão**: Incluir mensagens para erros de pesquisa, como "Nenhuma solicitação encontrada".

---

### Tela 5:
- **H6. Reconhecer ao invés de lembrar** (Severidade: 3)  
  - **Análise**: O usuário não sabe onde clicar para acessar os detalhes da solicitação.
  - **Sugestão**: Incluir um botão ou link visível para navegação.

---

### Tela 7:
- **H3. Controle e liberdade do usuário** (Severidade: 3)  
  - **Análise**: Não há uma opção para o usuário cancelar a tarefa.
  - **Sugestão**: Incluir um botão de "Cancelar".

---

## Consolidação dos Resultados

Os resultados indicam que o sistema apresenta uma série de violações das heurísticas de usabilidade, especialmente relacionadas ao feedback de erros e à liberdade do usuário. As recomendações feitas visam melhorar a interação e a usabilidade geral, com foco na prevenção de erros e na flexibilidade para os usuários.

## Recomendações Gerais
- **Validações**: Implementar validações de campos em tempo real em todas as telas.
- **Mensagens de Erro**: Fornecer mensagens de erro claras e detalhadas.
- **Navegação**: Garantir que o usuário tenha controle sobre suas ações, com botões de "Cancelar" e a opção de retornar às telas anteriores.
- **Ajuda e Documentação**: Adicionar seções de ajuda e suporte visíveis para melhorar a experiência do usuário.

