# Sistema de Reserva de Salas de Estudo Coletivo

Estrutura retirada do Sallas para o documento de visão

## 1. Objetivo do Projeto

O sistema **Reserva de Salas de Estudo Coletivo** tem como objetivo facilitar o gerenciamento das reservas das salas de estudo coletivo da Biblioteca do IFRN/CNAT. O sistema substituirá o método de reserva por fichas em papel, permitindo aos discentes e bolsistas uma gestão mais eficiente e facilitada, além de oferecer aos alunos a possibilidade de realizar reservas de salas online.

## 2. Descrição do Problema

| **Problema** | Falta de um sistema eficiente para gerenciar as reservas de salas de estudo coletivo, que atualmente é feito manualmente com fichas em papel. |
|--------------|-------------------------------------------------------------------------------------------------------|
| **Afetando** | Bolsistas, alunos e servidores do IFRN/CNAT. |
| **Impacto** | Dificuldade no controle das reservas, perda de fichas e falta de informações sobre a disponibilidade das salas. Para os alunos, a necessidade de ir até a biblioteca para saber se há salas disponíveis resulta em perda de tempo e frustração. |
| **Solução Proposta** | Desenvolver um sistema online onde os alunos possam verificar a disponibilidade das salas e fazer reservas de forma prática e rápida, enquanto os bolsistas e servidores podem gerenciar de forma mais eficiente e segura a utilização das salas. |

## 3. Descrição dos Usuários

| Nome     | Descrição                                                                 | Responsabilidades                                                                                 |
|----------|---------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| **Servidor** | Servidores responsáveis pela coordenação e administração das bibliotecas do campus. | Monitorar e fiscalizar as atividades dos bolsistas, analisar solicitações de reservas, gerenciar advertências aos alunos. |
| **Bolsista** | Estudantes do IFRN/CNAT que participam do programa de auxílio à formação estudantil e são responsáveis pela reserva das salas. | Controlar as reservas das salas, validar as pré-reservas, entregar kits e registrar possíveis problemas no sistema. |
| **Aluno** | Estudantes que frequentam a biblioteca e necessitam alugar as salas de estudo coletivo. | Realizar pré-reserva de salas e verificar a disponibilidade das salas online. |

## 4. Descrição do Ambiente dos Usuários

O sistema de reservas estará disponível online e acessível via navegador em qualquer dispositivo (computadores, tablets e smartphones). Os alunos podem verificar a disponibilidade das salas e realizar pré-reservas de forma online. Os bolsistas e servidores podem gerenciar as reservas e realizar as validações pessoalmente.

- **Servidor e Bolsista** terão acesso contínuo ao sistema para gerenciar as reservas, enquanto os **alunos** poderão acessar o sistema para consultar a disponibilidade e realizar reservas online durante o horário de funcionamento da biblioteca.
- **Ex-alunos** não terão acesso ao sistema, pois apenas discentes ativos da instituição poderão reservar as salas.

## 5. Principais Necessidades dos Usuários

- **Bolsistas** enfrentam dificuldades no gerenciamento das reservas com o uso de fichas em papel, o que gera perda de tempo e potencial para erros.
- **Alunos** necessitam de um meio para verificar a disponibilidade das salas sem precisar se deslocar fisicamente até a biblioteca, melhorando a experiência de utilização do espaço.
- **Servidores** precisam de um sistema para analisar e gerenciar as reservas de maneira mais eficiente e gerar relatórios para a administração.

A solução é um sistema online que facilita o processo de reserva e gerenciamento das salas, além de oferecer uma interface mais amigável e acessível.

## 6. Alternativas Concorrentes

- **Fichas de papel**:
  - Pontos fortes: Simples de entender e aplicar, não requer infraestrutura tecnológica.
  - Pontos fracos: Dificuldade na organização e risco de perdas de fichas, dificuldade em gerar relatórios e acessar informações de reservas em tempo real.

- **Planilhas (Excel ou similares)**:
  - Pontos fortes: Simples, ecológico, e permite a visualização clara das reservas.
  - Pontos fracos: Falta de automação em processos, risco de edição não autorizada e dificuldade de escalabilidade com o aumento de reservas.

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