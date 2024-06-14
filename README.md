## Analise Redes Sociais Show Madonna em Copacabana
![term_evolution_buzzmonitor](https://github.com/accperformance/madonna/assets/62457806/554d89a0-b701-4517-9833-c389feb23b27)
![shares_by_network](https://github.com/accperformance/madonna/assets/62457806/83a3cf79-4ee3-4b84-823c-f2f0720feff1)
![data_buzzmonitor_trends](https://github.com/accperformance/madonna/assets/62457806/4ccae58d-4acd-43bb-b5ba-59b6f4328ddd)
![sentiments_buzzmonitor_trends](https://github.com/accperformance/madonna/assets/62457806/1f721794-374f-4997-97b1-7648443dbb68)
![term_evolution_buzzmonitor (1)](https://github.com/accperformance/madonna/assets/62457806/98cbb2e3-696c-402e-8e2e-1b9a10c66d5c)
![shares_by_network (1)](https://github.com/accperformance/madonna/assets/62457806/f7103509-f236-4e1d-a87b-87ef429339e1)
![data_buzzmonitor_trends (1)](https://github.com/accperformance/madonna/assets/62457806/3435e76b-e551-411f-b3db-2311db793c41)
![sentiments_buzzmonitor_trends (1)](https://github.com/accperformance/madonna/assets/62457806/26a916d0-193e-4ef6-881f-db5775232b4a)
![term_evolution_buzzmonitor (2)](https://github.com/accperformance/madonna/assets/62457806/caccb682-07ea-4fd7-8d0b-a080ebd2cf38)
![shares_by_network (2)](https://github.com/accperformance/madonna/assets/62457806/087fdafb-4d69-4a69-abe5-7f62c305ebaa)
![data_buzzmonitor_trends (2)](https://github.com/accperformance/madonna/assets/62457806/86f6b714-836e-401e-9675-437d07301e58)
![sentiments_buzzmonitor_trends (2)](https://github.com/accperformance/madonna/assets/62457806/879ea722-81eb-42e6-87fe-8ee3f48e0138)
![term_evolution_buzzmonitor (3)](https://github.com/accperformance/madonna/assets/62457806/82f39bc3-6187-4e0c-92cc-5c35f252663c)
![shares_by_network (3)](https://github.com/accperformance/madonna/assets/62457806/638b913f-b70b-4f10-82fe-6a2fec4fde15)
![data_buzzmonitor_trends (3)](https://github.com/accperformance/madonna/assets/62457806/e487595f-a5b7-42bb-8408-7be7cf006dee)
![sentiments_buzzmonitor_trends (3)](https://github.com/accperformance/madonna/assets/62457806/ce948e69-57ca-48b0-a539-8478ed3b5592)

## Update de codigo> 20240614> apos reunião de 20240613 chagamos a conclusão da necessidade de atualizar os arquivos .csv com head, o label conter informações minimas para facilitar compreenção>> plataforma, data hora da publicação; normalização do formato do arquivo entre todas as plataformas para possivel analise cruzada ##

# Notas sobre conceito do codigo: #

Código Python em um Jupyter Notebook para realizar as seguintes tarefas:

Varrer os diretórios \madonna\face\, \madonna\Insta\ e \madonna\X\ em busca de arquivos .csv.
Criar a pasta \madonna\split caso ela não exista.
Ler cada arquivo .csv e gerar novos arquivos .csv onde cada linha original será um novo arquivo.
Nomear os novos arquivos com base na data, um número sequencial e o valor de sentimento.

Explicação:
Importações: Importamos as bibliotecas necessárias (os, pandas, datetime).
Diretórios: Definimos os diretórios de entrada e o diretório de saída.
Criação do Diretório de Saída: Utilizamos os.makedirs com exist_ok=True para criar a pasta \madonna\split se ela não existir.
Função get_sentiment_code: Função para mapear os sentimentos para seus respectivos códigos.
Processamento dos Arquivos:
Iteramos sobre os diretórios e arquivos .csv.
Para cada arquivo .csv, lemos o conteúdo e separamos o cabeçalho.
Iteramos sobre cada linha do DataFrame, gerando um novo nome de arquivo baseado na data atual, código de sentimento e número sequencial.
Salvamos cada linha como um novo arquivo .csv no diretório de saída.
Assumptions:
A coluna de sentimento no CSV se chama sentiment. Caso tenha outro nome, ajuste essa parte do código.
A estrutura dos arquivos .csv é conhecida e consistente.