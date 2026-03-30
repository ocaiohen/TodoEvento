# Sistema de cadastro em eventos

Estrutura retirada do Sallas para o documento de visão

## 1. Objetivo do Projeto

O sistema **TodoEvento** tem como objetivo facilitar a divulgação e inscrição em eventos do Instituto Federal do Rio Grande do Norte Campus Natal Central. O sistema resolve o problema da falta de divulgação de eventos que acontecem no campus. Organizadores poderão cadastrar eventos, ver estatísticas simples. Da mesma forma, participantes (visitantes no site) se cadastrarão usando a matrícula no evento.

## 2. Descrição do Problema

| **Problema** | Falta de uma divulgação modernizada e centralizada de evento do campus. |
|--------------|-------------------------------------------------------------------------------------------------------|
| **Afetando** | Participantes e organizadores. |
| **Impacto** | Perca de oportunidades de crescimento (ao não conhecer eventos interessantes) e pouco público em eventos. |
| **Solução Proposta** | Desenvolver um sistema online onde os organizadores cadastrariam eventos para os participantes se cadastrarem. |

## 3. Descrição dos Usuários

| Nome     | Descrição                                                                 | Responsabilidades                                                                                 |
|----------|---------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| **Organizador** | Organizadores (sejam externos ou internos) que desejam cadastrar e gerenciar eventos que ocorerrão no CNAT. | Cadastrar e gerenciar os próprios eventos
| **Participante** | Membros do IFRN/CNAT (sejam docentes ou discentes) que estejam interessados em procurar e se cadastrar em eventos. | Ver eventos e se cadastrar. |


## 4. Descrição do Ambiente dos Usuários

O sistema de eventos estará disponível online e acessível via navegador em qualquer dispositivo (computadores, tablets e smartphones).

- **Organizador** acesso livre às seções relativas ao gerenciamentos de seus próprios eventos.
- **Participante** acesso livre aos eventos cadastrados

## 5. Principais Necessidades dos Usuários

- **Organizador** cadastrar e gerenciar seus próprios eventos.
- **Participante** procurar e se cadastrar em eventos. 

## 6. Alternativas Concorrentes

- **Suap**:
  - Pontos fortes: já feito e usado pelos alunos.
  - Pontos fracos: não é feito para isso e muito menos divulgado.

## 7. Visão Geral do Produto

O sistema será acessado através de navegadores e permitirá que os alunos façam pré-reservas, enquanto os bolsistas gerenciem as reservas e validem as solicitações. O servidor terá acesso para monitorar e gerar relatórios.

O sistema terá três tipos de usuários principais:
- **Aluno**: Realiza pré-reservas e consulta disponibilidade de salas.
- **Bolsista**: Gerencia as reservas e validações, além de controlar as entregas de kits e monitorar o uso das salas.
- **Servidor**: Supervisiona as reservas e gera relatórios.

## 8. Requisitos Funcionais

| Código | Nome | Descrição |
|--------|------|----------|
| RF01 | Consultar disponibilidade de salas | O aluno poderá ver quais salas estão livres ou já reservadas. |
| RF02 | Realizar pré-reserva de salas | O aluno poderá pré-reservar uma sala de estudo coletivo online. |
| RF03 | Validar a reserva de sala | O bolsista poderá validar pessoalmente a reserva de sala, conforme o processo definido. |
| RF04 | Registrar observações | Bolsistas e alunos poderão registrar observações durante o processo de reserva. |
| RF05 | Verificar reservas anteriores | O bolsista e o servidor poderão acessar o histórico de reservas. |
| RF06 | Alterar responsável pela sala | O bolsista pode transferir a responsabilidade de uma reserva para outro membro. |
| RF07 | Criar advertências | O servidor poderá cadastrar advertências aos alunos que não cumprirem as regras de uso das salas. |
| RF08 | Atualizar status de utensílios da sala | O bolsista pode atualizar o status dos utensílios ou equipamentos disponíveis nas salas. |

## 9. Requisitos Não Funcionais

| Código | Nome | Descrição | Categoria | Classificação |
|--------|------|----------|-----------|---------------|
| RNF01 | Design responsivo | O sistema deve ser acessível em dispositivos de diferentes tamanhos de tela (computador, tablet, celular). | Usabilidade | Obrigatório |
| RNF02 | Privacidade | O sistema deve garantir a privacidade das informações dos usuários. | Segurança | Obrigatório |
| RNF03 | Facilidade de uso | O sistema deve ser intuitivo e fácil de usar para todos os usuários. | Usabilidade | Obrigatório |
| RNF04 | Acesso inclusivo | O sistema deve ser acessível a todos os usuários, independentemente de suas habilidades. | Acessibilidade | Obrigatório |
| RNF05 | Criptografia de dados | Todos os dados sensíveis devem ser armazenados de forma criptografada no banco de dados. | Segurança | Obrigatório |