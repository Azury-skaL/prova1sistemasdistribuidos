# prova1sistemasdistribuidos

Nome: Rafael Felipe Zambeli
RA: fc29b2a7a4e1e4246f65

##Problema da empresa

Foi necessário criar um código para uma empresa que necessitava de um serviço dedesconto, o cliente deve solicitar ao servidor e o mesmo deve realizar o calculo

## Arquivos

servidor.py: recebe a chamada RPC e executa o calculo.
cliente.py: solicita o cálculo ao servidor e mostra a resposta.

## Resultado do teste

PS C:\Users\aluno\Desktop\prova1 sistemas distribuidos> 










                                                      > & "C:\Program Files\Python313\python.exe" "c:/Users/aluno/Desktop/prova1 sistemas distribuidos/cliente.py"
Traceback (most recent call last):
  File "c:\Users\aluno\Desktop\prova1 sistemas distribuidos\cliente.py", line 5, in <module>
    resultado = servidor.calcular_desconto(200, 10)
  File "C:\Program Files\Python313\Lib\xmlrpc\client.py", line 1096, in __call__
    return self.__send(self.__name, args)
           ~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^
  File "C:\Program Files\Python313\Lib\xmlrpc\client.py", line 1435, in __request
    response = self.__transport.request(
        self.__host,
    ...<2 lines>...
        verbose=self.__verbose
        )
  File "C:\Program Files\Python313\Lib\xmlrpc\client.py", line 1140, in request
    return self.single_request(host, handler, request_body, verbose)
           ~~~~~~~~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Program Files\Python313\Lib\xmlrpc\client.py", line 1152, in single_request
    http_conn = self.send_request(host, handler, request_body, verbose)
  File "C:\Program Files\Python313\Lib\xmlrpc\client.py", line 1265, in send_request
    self.send_content(connection, request_body)
    ~~~~~~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Program Files\Python313\Lib\xmlrpc\client.py", line 1295, in send_content
    connection.endheaders(request_body)
    ~~~~~~~~~~~~~~~~~~~~~^^^^^^^^^^^^^^
  File "C:\Program Files\Python313\Lib\http\client.py", line 1333, in endheaders
    self._send_output(message_body, encode_chunked=encode_chunked)
    ~~~~~~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Program Files\Python313\Lib\http\client.py", line 1093, in _send_output
    self.send(msg)
    ~~~~~~~~~^^^^^
  File "C:\Program Files\Python313\Lib\http\client.py", line 1037, in send
    self.connect()
    ~~~~~~~~~~~~^^
  File "C:\Program Files\Python313\Lib\http\client.py", line 1003, in connect
    self.sock = self._create_connection(
                ~~~~~~~~~~~~~~~~~~~~~~~^
        (self.host,self.port), self.timeout, self.source_address)
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Program Files\Python313\Lib\socket.py", line 864, in create_connection
    raise exceptions[0]
  File "C:\Program Files\Python313\Lib\socket.py", line 849, in create_connection
    sock.connect(sa)
    ~~~~~~~~~~~~^^^^
ConnectionRefusedError: [WinError 10061] Nenhuma conexão pôde ser feita porque a máquina de destino as recusou ativamente
PS C:\Users\aluno\Desktop\prova1 sistemas distribuidos> 

## Explicação
1. Em qual programa o cálculo foi executado
   R: Foi executado no servidor.
2. Qual programa iniciou a colicitação?
   R: O cliente
3. O que aconteceria com o cliente se o servidor estivesse desligado?
   R: O cálculo não iria rodar e uma mensagem de erro seria apresentada.    
