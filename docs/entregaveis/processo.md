Documentos de Processo e Definição

Estes documentos contêm a "inteligência" da planta. Eles definem as regras de operação e controle.

1. Fluxograma de Engenharia (P&ID)

O documento mais importante do projeto. No executivo, ele deve conter:

Tagueamento completo de todos os instrumentos.

Diâmetros de tubulação e especificação de material.

Intertravamentos lógicos representados (Losangos de lógica).

Drenos, vents e conexões de purga.

Limites de Bateria: Onde termina o escopo do projeto.

2. Folhas de Dados (Data Sheets)

O documento de compra. Deve ser separado por tipo de instrumento (ex: FD para Transmissores de Pressão, FD para Válvulas de Controle).

Conteúdo Obrigatório:

Dados de Processo: Fluido, Pressão (Min/Norm/Máx), Temperatura, Densidade, Viscosidade.

Dados Construtivos: Material do corpo, material do sensor (diafragma), conexões (1/2" NPT), grau de proteção (IP66).

Dados Elétricos: Alimentação (24Vdc), Sinal de Saída (4-20mA HART), Classificação de Área (Ex i, Ex d).

3. Matriz de Causa e Efeito

Define a lógica de segurança e intertravamento de forma tabular, legível para humanos e programadores.

Tag (Causa)

Descrição

Setpoint

...

XV-01 (Efeito)

Bomba-01 (Efeito)

Sirene (Efeito)

PIT-101

Pressão Alta Tanque

> 5 Bar

...

X (Fechar)

X (Desligar)

X (Ligar)

LIT-200

Nível Baixo Tanque

< 10%

...

-

X (Desligar)

-

4. Memorial Descritivo

Texto corrido explicando a filosofia de controle.

"O controle de nível será feito por uma malha PID atuando na vazão de entrada..."

"O sistema de emergência atuará desenergizando as solenoides (Fail Safe)..."