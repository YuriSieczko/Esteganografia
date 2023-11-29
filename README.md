# Esteganografia
Para decodificar a mensagem:

Análise das Cores: Cada cor na página é representada em valores hexadecimais no formato #RRGGBB (Red, Green, Blue).

Identificação da Codificação: A mensagem está codificada na parte menos significativa das cores. As duas primeiras cores foram modificadas para representar a mensagem.

Decodificação da Mensagem:

Vermelho (#FF0000): O valor foi alterado de #FF0000 para #FF0101 para representar a letra "Y" (89 em ASCII).

Verde (#00FF00): O valor foi alterado de #00FF00 para #00FF10 para representar a letra "u" (117 em ASCII).

Azul (#0000FF): Mantido sem alterações.

Conversão para ASCII: Converta cada conjunto de bits alterados (8 bits para cada letra) de binário para decimal e depois para ASCII para recuperar a mensagem original.

Vermelho alterado: #FF0101 => (01011001 => 89 em decimal) = "Y"
Verde alterado: #00FF10 => (01110101 => 117 em decimal) = "u"
Azul inalterado: #0000FF => (letra "r" ou "i" não foi modificada)