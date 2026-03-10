# Casos de Teste - API ViaCEP

## CT01 - Consulta um CEP válido
Dado que o usuário acessa a API ViaCEP  
Quando digita o CEP 01001000  
Então a API retorna status 200  
E retorna os dados do endereço corretamente

## CT02 - Consulta CEP inexistente
Dado que o usuário digita o CEP 00000000  
Então a API retorna erro=true

## CT03 - CEP inválido
Dado que o usuário digita um CEP inválido  
Então a API retorna um erro
