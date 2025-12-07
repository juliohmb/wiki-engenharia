Comissionamento e Validação

O projeto executivo deve prever documentos que suportem a fase de testes, garantindo que o que foi projetado funciona.

1. FAT (Factory Acceptance Test)

Teste de Aceitação em Fábrica. Ocorre no galpão do integrador, antes de enviar os painéis para a obra.

Visual/Dimensional: O painel segue o desenho? A pintura está ok?

Energização: As fontes funcionam? Não há curto-circuito?

Lógica (Simulação): Injeta-se sinais simulados no cartão do CLP e verifica-se se a lógica e o supervisório respondem conforme a Matriz de Causa e Efeito.

2. SAT (Site Acceptance Test)

Teste de Aceitação em Campo. Verifica se o equipamento chegou inteiro após o transporte.

Re-aperto de bornes.

Verificação de danos físicos.

Energização preliminar.

3. Loop Check (Verificação de Malha)

O teste mais importante da instrumentação.

Cold Loop Check: Teste de continuidade ("Bipar" o cabo) do campo até o painel, sem energia. Garante que o par + do instrumento X chega no borne + do cartão X.

Hot Loop Check: Com o sistema energizado, simula-se 4mA (0%) e 20mA (100%) no transmissor e verifica-se a leitura na tela de operação.

4. TAF e TAC

Conforme norma NBR IEC 62381:

TAF: Teste de Aceitação em Fábrica.

TAC: Teste de Aceitação em Campo.

!!! info "Pasta de Comissionamento"
Cada malha deve ter sua "Folha de Teste de Malha" assinada, contendo: Tag, Data, Leitura Esperada vs. Leitura Real, e assinatura do responsável.