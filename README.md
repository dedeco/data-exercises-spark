
## Introdução

Uma startup de streaming de música, Sparkify, aumentou sua base de usuários e banco de dados de músicas ainda mais e deseja mover seu data warehouse para um data lake. Seus dados residem no S3, em um diretório de logs JSON na atividade do usuário no aplicativo, bem como em um diretório com metadados JSON nas músicas em seu aplicativo.

## Datasets

Você trabalhará com dois conjuntos de dados que residem no S3. Aqui estão os links S3 para cada: 

- Song data: s3://udacity-dend/song_data
- Log data: s3://udacity-dend/log_data

### Song Dataset

O primeiro conjunto de dados é um subconjunto de dados reais do Conjunto de dados do milhão de canções. Cada arquivo está no formato JSON e contém metadados sobre uma música e o artista dessa música. Os arquivos são particionados pelas três primeiras letras do ID da faixa de cada música. Por exemplo, aqui estão os caminhos de arquivo para dois arquivos neste conjunto de dados.

```
song_data/A/B/C/TRABCEI128F424C983.json
song_data/A/A/B/TRAABJL12903CDCF1A.json
```

E abaixo está um exemplo da aparência de um único arquivo de música, TRAABJL12903CDCF1A.json.

```
{"num_songs": 1, "artist_id": "ARJIE2Y1187B994AB7", "artist_latitude": null, "artist_longitude": null, "artist_location": "", "artist_name": "Line Renaud", "song_id": "SOUPIRU12A6D4FA1E1", "title": "Der Kleine Dompfaff", "duration": 152.92036, "year": 0}
```

### Log Dataset

O segundo conjunto de dados consiste em arquivos de log no formato JSON gerados por este simulador de eventos com base nas músicas do conjunto de dados acima. Eles simulam registros de atividades de aplicativos de um aplicativo de streaming de música imaginário com base nas definições de configuração.

Os arquivos de log no conjunto de dados com o qual você trabalhará são particionados por ano e mês. Por exemplo, aqui estão os caminhos de arquivo para dois arquivos neste conjunto de dados.

```
log_data/2018/11/2018-11-12-events.json
log_data/2018/11/2018-11-13-events.json
```

Para outros desafios vamos usar esses datasets:

- Full Sparkify Dataset: s3n://udacity-dsnd/sparkify/sparkify_event_data.json (12Gb)
- Medium: https://video.udacity-data.com/topher/2018/December/5c1d6681_medium-sparkify-event-data/medium-sparkify-event-data.json


# Como fazer os exercícios?

Você irá dar um [fork](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo) nesse repositório na sua máquina. Depois você irá [clonar o seu repositório](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) na sua conta do github e ao terminar commitar as alterações no notebook e subir, ou seja [dar um push](https://docs.github.com/pt/github/using-git/pushing-commits-to-a-remote-repository).

E então abrir [um pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) para revisarmos as respostas

## Exercício 1

Na pasta /data tem uma pequena amostra do dataset para exploração do primeiro exercício. Na pasta exerc01 tem o notebook no qual vc deverá responder no próprio notebook as respostas esperadas para cada pergunta.


# Agradecimento
Obrigado a Udacity pelo uso e compartilhamento do DATASET.



