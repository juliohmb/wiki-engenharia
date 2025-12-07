IEC: Estruturas de Controle e Segurança

Enquanto a ISA cuida da representação, a IEC cuida da lógica e da segurança elétrica.

IEC 61131-3: Linguagens de Programação

Padroniza como os CLPs (Controladores Lógicos Programáveis) são programados. Um projeto executivo deve definir qual linguagem será usada para facilitar a manutenção.

Ladder Diagram (LD): Lógica de relés. Padrão para intertravamentos e manutenção elétrica.

Function Block Diagram (FBD): Blocos visuais. Padrão para controle de processo contínuo (PIDs) e instrumentação.

Structured Text (ST): Similar a Pascal/C. Usado para cálculos complexos e manipulação de dados.

Sequential Function Chart (SFC): Grafcet. Usado para processos em batelada (sequenciais).

Instruction List (IL): (Em desuso) Similar a Assembly.

IEC 62443: Cibersegurança Industrial (IACS)

No mundo da Indústria 4.0, a segurança cibernética é um requisito de projeto, não um "adicional".

Conceitos Fundamentais

Defesa em Profundidade (Defense in Depth): Múltiplas camadas de proteção.

Zonas e Condutos: Agrupar ativos com requisitos de segurança similares em "Zonas" e controlar a comunicação entre elas via "Condutos" (Firewalls industriais).

!!! danger "Segurança por Obscuridade"
Nunca confie que "ninguém sabe o IP do meu CLP" como medida de segurança. Projetos modernos exigem segmentação de rede (VLANs) e controle de acesso rigoroso.

IEC 61511: Segurança Funcional (SIS)

Aplica-se quando a falha do sistema pode causar danos a vidas ou ao meio ambiente.

Define o SIL (Safety Integrity Level): Probabilidade de falha sob demanda.

Um instrumento SIS (Ex: Trip de Pressão Alta) deve ser independente do sistema de controle regulatório (BPCS).