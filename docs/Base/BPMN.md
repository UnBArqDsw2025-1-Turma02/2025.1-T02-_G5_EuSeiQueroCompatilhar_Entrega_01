# Projeto de Plataforma de Guias de Jogos - Modelagem BPMN

## Introdução

## Metodologia

A modelagem BPMN da arquitetura da plataforma de guias de jogos seguiu uma abordagem dividida em etapas:

### Levantamento de Processos (AS-IS)

Foram identificados os principais processos relacionados à experiência do usuário, como registro/login, submissão de guia, leitura e avaliação de conteúdo. Também foram definidos os papéis de usuário (criador de conteúdo, leitor ou ambos), considerando também o processo de verificação/insígnia para diferenciar empresas de usuários comuns.

### Modelagem BPMN

Utilizando ferramentas como Bizagi ou Camunda, os fluxos foram representados graficamente. Foram modelados, por exemplo, os fluxos de submissão de guias (com etapas de escrita, revisão e publicação), leitura e avaliação por outros usuários (incluindo comentários e notas), e verificação de conta (solicitação, análise e concessão de insígnias).

### Análise Técnica

Com os modelos definidos, foi possível identificar os pontos de integração entre os módulos do sistema, como o serviço de autenticação (login), o banco de dados de guias, e o serviço de avaliação e comentários. Além disso, foram levantadas as APIs necessárias para suportar funcionalidades como exibição de rankings de guias, recomendações personalizadas e controle de permissões por tipo de usuário.

### Modelagem TO-BE e Transformação

A versão futura do sistema (TO-BE) foi projetada para escalar conforme o crescimento da base de usuários e conteúdo. A proposta contempla modularização via microserviços, uso de filas de eventos para notificações e comentários em tempo real, e aplicação de práticas como DevOps para integração contínua. Isso garante a evolução sustentável da plataforma, mantendo sua usabilidade e desempenho.

## Conclusão

A utilização da modelagem BPMN na concepção da plataforma de comunidade de guias de jogos permitiu uma visualização clara e precisa dos processos principais da aplicação. A representação dos fluxos de submissão, leitura e avaliação de guias, além da diferenciação entre tipos de usuários, contribuiu para um entendimento unificado entre equipe técnica e stakeholders. Como resultado, foi possível desenhar uma arquitetura escalável, orientada a serviços e adaptada às necessidades reais da comunidade gamer. Essa abordagem garante uma base sólida para a construção de um sistema colaborativo, engajador e tecnicamente eficiente.

## Refêrencias

Aprender 3: Acesso ao site. Disponível em: <https://aprender3.unb.br/pluginfile.php/3070931/mod_page/content/2/Arquitetura%20e%20Desenho%20de%20software%20-%20Aula%20BPMN%20Exemplos%20-%20Profa.%20Milene.pdf>. Acesso em: 11 abr. 2025.

WHITE, Stephen A.
Business Process Modeling Notation (BPMN) – Version 1.0.
BPMI.org, 2004.

ROZANSKI, Nick; WOODS, Eóin.
Software Systems Architecture: Working with Stakeholders Using Viewpoints and Perspectives.
Addison-Wesley, 2011.

HILL, Charles W. L.; JONES, Gareth R.
Strategic Management Theory: An Integrated Approach.
Cengage Learning, 2012.

BASS, Len; CLEMENTS, Paul; KAZMAN, Rick.
Software Architecture in Practice.
Addison-Wesley, 2012.

FIELDING, Roy T.
Architectural Styles and the Design of Network-based Software Architectures.
Tese de doutorado, University of California, 2000.

WENGER, Etienne.
Communities of Practice: Learning, Meaning, and Identity.
Cambridge University Press, 1998.

## Histórico de versão:

| Versão | Alteração                    | Responsável     | Revisor | Data       | Detalhes da Revisão |
|--------|------------------------------|------------------|---------|------------|----------------------|
| 1.0    | Elaboração do documento      | [Fernando Gabriel](https://github.com/show-dawn) e [Vitor](https://github.com/vcpVitor) |         | 10/04/2025 | Versão inicial conclusão BPMN |
| 1.0    | Adiciona metodologia e refêrencias      | [Júlio Cesar](https://github.com/Julio1099) e [Matheus Ferreira](https://github.com/matferreira1) |         | 11/04/2025 | Versão inicial metodologia BPMN |