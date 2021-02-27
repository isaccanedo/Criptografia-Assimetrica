# Criptografia-Assimetrica
:computer: # Criptografia Assimétrica

## Aprenda o que é criptografia assimétrica, como funciona e o que faz

Quando se trata da palavra "criptografia", pensamos nela como uma técnica que protege dados usando uma chave criptográfica, e não há nada de errado com isso. No entanto, o que a maioria das pessoas não percebe é que existem diferentes tipos de métodos de criptografia. A criptografia assimétrica, também conhecida como criptografia de chave pública, é um exemplo de um tipo.

Ao contrário da criptografia “normal” (simétrica), a criptografia assimétrica criptografa e descriptografa os dados usando duas chaves criptográficas separadas, mas conectadas matematicamente. Essas chaves são conhecidas como ‘Chave Pública’ e ‘Chave Privada’. Juntas, são chamadas de ‘Par de Chaves Públicas e Privadas’.

Vamos ver como essas duas chaves funcionam juntas para criar a força formidável que é a criptografia assimétrica.

## Como funciona a criptografia assimétrica?
A criptografia assimétrica usa duas chaves distintas, mas relacionadas. Uma chave, a chave pública, é usada para criptografia e a outra, a chave privada, é usada para descriptografar. Conforme implícito no nome, a chave privada deve ser privada para que apenas o destinatário autenticado possa descriptografar a mensagem.

Vamos entender isso com um exemplo simples de criptografia assimétrica.

Finja que você é uma agência de espionagem e precisa criar um mecanismo para seus agentes se reportarem com segurança. Você não precisa de comunicação bidirecional, eles têm seus pedidos, você só precisa de relatórios regulares detalhados vindos deles. A criptografia assimétrica permitiria a criação de chaves públicas para os agentes criptografarem suas informações e uma chave privada na sede, que é a única maneira de descriptografar tudo. Isso fornece uma forma impenetrável de comunicação unilateral.

<img src="asymmetric-encryption.png">

## Como as duas chaves são geradas?
No coração da criptografia assimétrica está um algoritmo criptográfico. Este algoritmo usa um protocolo de geração de chave (um tipo de função matemática) para gerar um par de chaves. Ambas as teclas estão matematicamente conectadas uma com a outra. Essa relação entre as chaves difere de um algoritmo para outro.

O algoritmo é basicamente uma combinação de duas funções - função de criptografia e função de descriptografia. Para afirmar o óbvio, a função de criptografia criptografa os dados e a função de descriptografia os descriptografa.

## É assim que a criptografia assimétrica é usada em certificados SSL/TLS
Em SSL / TLS e outros certificados digitais, ambos os métodos - simétrico e assimétrico - são empregados. Agora, você deve estar se perguntando: 'Por que ambos? A criptografia assimétrica não deveria ser usada por ser mais segura? "Com certeza, é mais segura, mas vem com uma armadilha. Uma grande desvantagem quando se trata de criptografia de chave pública é o tempo computacional. Como a verificação e as funções são aplicadas de ambos os lados, isso retarda o processo significativamente. É aí que a criptografia simétrica vem e salva o dia.

Primeiro, quando duas partes (navegador e servidor, no caso de SSL) se cruzam, elas validam a chave privada e pública uma da outra por meio da criptografia assimétrica. Assim que a verificação for bem-sucedida e ambos souberem com quem estão falando, a criptografia dos dados será iniciada - por meio da criptografia simétrica. Economizando assim um tempo significativo e atendendo aos propósitos de confidencialidade e proteção de dados. Todo esse processo é chamado de handshake SSL/TLS. 


Opts are set via environment variables

| Criptografia simétrica                                   | Criptografia Assimétrica                                         |
|----------------------------------------------------------|------------------------------------------------------------------|
| A criptografia simétrica consiste em uma das chaves      | A criptografia assimétrica consiste em duas chaves               |
| para criptografia e descriptografia.                     | criptográficas conhecidas como chave pública e chave privada.    |
|----------------------------------------------------------|------------------------------------------------------------------|

| A criptografia simétrica é muito mais rápida em          | Como a criptografia assimétrica incorpora duas chaves separadas, | 
| comparação com o método assimétrico.                     | o processo fica consideravelmente mais lento.
|                                                          |
| RC4                                                      | RSA
|                                                          |
| AES                                                      | Diffie-Hellman
| 
| DES
|
| 3DES
|
| QUAD
