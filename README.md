# DataEngineerKeyCash

Teste proposto para a vaga de Engenheiro de Dados Jr. na Key Cash:

Seu desafio é:

1- Criar um script Python que faz a ingestão de 50 arquivos semi-estruturados em um storage cloud (exemplo: AWS S3, Google Cloud Storage). https://keycash-mkt.s3.amazonaws.com/vagas/Data-Engineer-Challenge.zip



2-Você deve ingerir todas as informações dos arquivos do Storage em uma tabela chamada LANDING_TABLE em seu DataWarehouse (DW) (Exemplo: Snowflake, Redshift, BIGQUERY). Você pode fazer isso de duas formas:

2.1: Para cada arquivo ingerido no Storage, um trigger é disparado e insere linhas na tabela LANDING_TABLE no DW.

2.2: Um trigger com horário pré-definido no DW é disparado e copia todos os arquivos/dados, DE UMA VEZ, criando a tabela LANDING_TABLE no DW.



NOTA: A tabela LANDING_TABLE deve conter todas as informações dentro dos arquivos .json



3-A partir da tabela LANDING_TABLE do DW você deve construir uma segunda tabela, também dentro do DW, chamada CREDIT_PER_DAY, agregando o somatório de Crédito Solicitado (credito_solicitado) por dia (data_solicitada). Lembre-se de que alguns clientes podem ter solicitado crédito mais de uma vez e APENAS a solicitação mais recente é válida.



4-Por fim, você deve conectar o seu DW à alguma ferramente de BI de sua preferência, criando uma visualização da tabela CREDIT_PER_DAY.



Outras informações importantes:

- Você tem uma semana para resolver este desafio e após esta data deve nos enviar uma apresentação mostrando como resolveu o problema e iremos agendar uma reunião para que você nos apresente a sua solução.

- Não se preocupe caso não consiga terminar todo o desafio.

-Tente pelo menos nos apresentar qual seria a sua solução final. Atente-se ao objetivo principal, mas sinta-se a vontade para implementar outros passos no pipeline, como testes de qualidade e outras visualizações.

- Use recursos visuais como diagramas (ex: draw.io) para facilitar a sua apresentação.

- Para facilitar o compartilhamento dos códigos desenvolvidos durante o desafio, você pode fazer upload dos arquivos em um repositório git.

