ISA 5.1: Simbologia e Identificação

A norma ANSI/ISA-5.1 estabelece um método uniforme para designar instrumentos e sistemas de instrumentação. Sem ela, um P&ID é apenas um desenho artístico sem valor técnico.

Estrutura do Tag

Um tag típico de instrumento carrega informações de Variável e Função.

TIT-101A

T (1ª Letra): Variável Medida -> Temperature (Temperatura).

I (Letra Sucessiva): Função de Informação -> Indication (Indicador).

T (Letra Sucessiva): Função de Saída -> Transmitter (Transmissor).

101 (Numeração): Identificação da malha (Área + Sequencial).

A (Sufixo): Diferenciador (ex: redundância ou instrumentos paralelos).

Tabela Resumida de Letras (Comuns)

Letra

1ª Letra (Variável)

Letras Sucessivas (Função)

A

Analysis (Análise)

Alarm (Alarme)

F

Flow (Vazão)

-

L

Level (Nível)

Light (Lâmpada Piloto)

P

Pressure (Pressão)

-

T

Temperature (Temperatura)

Transmitter (Transmissor)

V

Vibration / Valve

Valve (Válvula)

I

Current (Corrente)

Indicator (Indicador)

C

-

Controller (Controlador)

S

Speed (Velocidade)

Switch (Chave)

Y

Event / State

Relay/Computing (Conversor/Relé)

Z

Position (Posição)

Element (Atuador/Elemento Final)

Simbologia Gráfica (Balloons)

A localização e acessibilidade do instrumento são definidas pelo símbolo gráfico.

Círculo Simples: Montado no campo (local), acessível ao operador.

Círculo dentro de Quadrado: Display compartilhado/Controle Distribuído (SDCD/CLP).

Hexágono: Função de Computador / Lógica de Software.

Linha Tracejada no Centro: Montado atrás do painel (não acessível ao operador).

Tipos de Linhas de Conexão

É crucial diferenciar os sinais no diagrama:

_______ Processo: Tubulação principal.

------- Elétrico: Sinal analógico (4-20mA) ou discreto (24Vdc).

// // Pneumático: Sinal de ar comprimido (para válvulas).

o--o--o Data Link: Comunicação digital (Fieldbus, Ethernet, Modbus).

x--x--x Capilar: Tubo capilar preenchido (selo remoto).

Exemplo de Malha Típica

graph LR
    A((FE-101)) -->|Processo| B((FIT-101))
    B -.->|4-20mA| C(FIC-101)
    C -.->|4-20mA| D(FY-101)
    D == Ar ==>// E((FV-101))
    
    style C fill:#f9f,stroke:#333,stroke-width:2px
    style D fill:#ff9,stroke:#333,stroke-width:2px


FE-101: Elemento de Vazão (Placa de Orifício).

FIT-101: Transmissor de Vazão.

FIC-101: Controlador Indicador de Vazão (No SDCD).

FY-101: Posicionador / Conversor I/P.

FV-101: Válvula de Controle.