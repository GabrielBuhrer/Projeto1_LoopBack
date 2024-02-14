No console python, 'pip install pyserial'
Verificar em gerenciador qual porta com esta o aduino 
Talvez mudar a porta usb. Ou tirar e por quando nao tem autorizacao :-\

getBufferLen:
    tamanho do buffer atual (quantos bytes estão atualmente armazenados)

getAllBuffer:
    retorna os bytes armazenados no buffer

getBuffer:
    retornar os primeiro "nData" bytes do buffer

getNData:
    quando uma determinada quantidade de bytes estiverem no buffer,eles são retornados (utilizando o getBuffer)

clearBuffer:
    limpa o buffer

sendBuffer:
    inicializa ou redefine transLen (saber o comprimento dos dados transmitidos)
    variável buffer recebe os dados forneciidos (bytes que serão enviados pela camada de transmissão)
    se thread está ativo, indica que a transmissão está pronta para começar
    em resumo: prepara a camada de transmissão para enviar os dados como argumento, dpois reinicia o rastreamento
        do tamanho da transmissão e configura a thread para que a transmissão seja iniciad