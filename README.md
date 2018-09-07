# sped-efd

## EM DESENVOLVIMENTO !!! não util ...

Classes para a geração do SPED EFD (fiscal ICMS IPI) e para o SPED EFD contribuições

## IMPORTANTE

- A finalidade desse projeto é APENAS fornecer os meios para criar os arquivos EFD ICMS/IPI e contribuições a partir de dados formecidos pelo sistema ERP.
- É necessario que os dados já estejam previamente tratados e consolidados internamente no ERP antes da geração dos arquivos de transmissão.
- Para entender o processo de montagem dos arquivos de envio, é OBRIGATÓRIO o conhecimento sobre esses dados e o estudo da documentação da Receita Federal. 
- Haverão centenas de classes !!! uma para cada elemento de um bloco, esses elementos poderão ser unicos, varios, obrigatórios ou não dependendo de uma série de condições, que não serão gerenciadas por esse construtor.
- O processo de montagem dos blocos é complexo e irá requerer tempo de processamento e memória, tendo em vista o volume de dados que poderá existir.  
- Após a geração do arquivo o mesmo deve ser validado pelo validador oficial da Receita e transmitido pelo Receitanet, não é possivel a validação automática nem o envio automatico por webservice


## Detalhes dos Campos

Todos os campos "C" strings apenas com caracteres ASCII, não são permitidos outro charsets, preferencialmente em "MAIUSCULAS"

Todos os campos "N" apenas numericos como:

$ 1.129.998,99 => 1129998,99

1.255,42 => 1255,42

234,567 => 234,567

10.000 => 10000

10.000,00 => 10000 ou 10000,00

17,00 % => 17,00 ou 17

18,50 % => 18,5 ou 18,50

30 => 30

1.123,456 Kg => 1123,456

0,010 litros => 0,010

0,00 => 0 ou 0,00

0 => 0

campo vazio => 

Observando o numero de decimais em cada caso

