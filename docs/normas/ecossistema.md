O Ecossistema Normativo

A instrumentação industrial no Brasil opera em um cenário híbrido, misturando normas americanas (pela influência do petróleo), europeias (pela segurança e elétrica) e nacionais.

Pirâmide de Normas

graph TD
    A[Lei Nacional / NR-10 / NR-12] --> B[Normas Brasileiras NBR]
    B --> C[Normas Internacionais ISA / IEC]
    C --> D[Normas de Cliente / PETROBRAS N]


Principais Entidades

1. ISA (International Society of Automation)

Focada na Linguagem e Funcionalidade.

ISA 5.1: Símbolos e Identificação (A "língua" do P&ID).

ISA 5.4: Diagramas de Malha.

ISA 20: Especificação de Instrumentos (Data Sheets).

2. IEC (International Electrotechnical Commission)

Focada na Elétrica, Segurança e Hardware.

IEC 61131: Linguagens de programação de CLP.

IEC 61508 / 61511: Segurança Funcional (SIS/SIL).

IEC 60529: Graus de Proteção (IP).

3. ABNT (Brasil)

Adapta as normas internacionais para a realidade legal brasileira.

NBR 5410: Instalações elétricas de baixa tensão (aplica-se à infraestrutura).

Série NBR IEC 60079: Atmosferas Explosivas (Ex).

NBR 10300: Cabos de instrumentação com blindagem.

4. Normas de Cliente (Ex: Petrobras)

Muitas vezes, tornam-se o padrão de fato do mercado devido ao nível de exigência.

N-1882: Critérios para Elaboração de Projetos de Instrumentação.

N-1883: Apresentação de Projetos de Instrumentação.

!!! tip "Dica de Projeto"
Sempre verifique a Folha de Dados de Projeto (Project Data) do cliente antes de iniciar. Ela define qual norma prevalece em caso de conflito. Normalmente: Lei > Norma Cliente > NBR > Norma Internacional.