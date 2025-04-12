# Projeto de Plataforma de Guias de Jogos - Modelagem BPMN

## Introdução

Segundo [(SERRANO)](#refêrencias), a Business Process Management Notation (BPMN) é uma notação padronizada para diagramação de fluxos de processos de negócio, adotada pelo consórcio internacional Object Management Group (OMG). Essa notação visa proporcionar uma representação gráfica clara e unificada dos processos, facilitando a comunicação entre stakeholders técnicos e não técnicos.

A BPMN utiliza elementos como piscinas (pools), raias (lanes), atividades, eventos, gateways e conectores para modelar desde processos simples até fluxos complexos, incluindo subprocessos e reutilização de atividades (Serrano, 2019). Entre seus principais componentes destacam-se:

- Piscinas/POOL: representam participantes do processo (internos ou externos);

- Raias/LANE: organizam atividades por papéis ou departamentos;

- Gateways: controlam divergências e convergências de fluxos (exclusivos, inclusivos, paralelos);

- Eventos: marcam ocorrências que influenciam o processo (início, fim, intermediários).

A notação é amplamente utilizada para mapear, analisar e melhorar processos organizacionais, sendo essencial para implementações de BPM (Business Process Management). Para Serrano (2019), a prática constante de modelagem é fundamental para dominar a BPMN, aliando teoria a exemplos concretos.

## Metodologia

O BPMN principal do projeto se apresenta a seguir:

![bpmn](/docs/Imagens/bpnm.png)
**Figura 1**: BPMN do projeto Backseat. **Autores**: Rodrigo Orlandi, João Marques

![](/docs/Imagens/BPMN-Login.png)
**Figura 2**: BPMN do Login. **Autores**: Rodrigo Gontijo, Henrique Galdino

![](/docs/Imagens/BPMN-Moderar.png)
**Figura 3**: BPMN do Moderar. **Autores**: Rodrigo Gontijo, Henrique Galdino

A modelagem BPMN da arquitetura da plataforma de guias de jogos seguiu uma abordagem dividida em etapas:

### Levantamento de Processos (AS-IS)

Foram identificados os principais processos relacionados à experiência do usuário, como login, submissão de guia, leitura e avaliação de conteúdo. Também foram definidos os papéis como usuário e moderador. Apesar de não representado visualmente, foi considerado também o processo de verificação/insígnia para diferenciar empresas de usuários comuns.

### Modelagem BPMN

Utilizando o Miro como ferramenta principal, os fluxos foram representados graficamente. Foram modelados os fluxos de submissão de guias (com etapas de escrita, revisão e publicação), leitura e pesquisa. O fluxo de visualização de guias leva a avaliação por outros usuários (incluindo comentários e notas), submissão de comentários e reportar guias potencialmente inadequados. A partir de guias reportados, os moderadores podem decidir moderar o guia, o que leva a outro BPMN que, infelizmente, não foi modelado nessa entrega.

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

HILL, Charles W. L.; JONES, Gareth R.
Strategic Management Theory: An Integrated Approach.
Cengage Learning, 2012.

ROZANSKI, Nick; WOODS, Eóin.
Software Systems Architecture: Working with Stakeholders Using Viewpoints and Perspectives.
Addison-Wesley, 2011.

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
| 1.1    | Adiciona metodologia e refêrencias      | [Júlio Cesar](https://github.com/Julio1099) e [Matheus Ferreira](https://github.com/matferreira1) |         | 11/04/2025 | Versão inicial metodologia BPMN |
| 1.2    | Adiciona introdução BPMN      | [João Paulo Monteiro](https://github.com/joaombc) e [Igor Santana][https://github.com/iGor-thiago] |         | 11/04/2025 | Versão inicial metodologia BPMN |
| 1.3    | Adicionado Diagrama BPNM, corrigido texto | [Rodrigo Orlandi](https://github.com/orlandirodrigo) e [João Marques][https://github.com/jmarquees] |         | 11/04/2025 | Versão inicial metodologia BPMN |
| 1.4    | Adicionado Diagramas BPNM restantes |  [Rodrigo Gontijo](https://github.com/rodrigogontijoo) e [Henrique Galdino][https://github.com/hgaldino05] |         | 11/04/2025 | |