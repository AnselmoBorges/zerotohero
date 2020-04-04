| [Home](https://techlipe.github.io/Workshop-Zero-To-Hero) | [Dia 01](https://techlipe.github.io/Workshop-Zero-To-Hero/dia01-configuracoes) | [Dia 02](https://techlipe.github.io/Workshop-Zero-To-Hero/dia02-observabilidade) | [Dia 03](https://techlipe.github.io/Workshop-Zero-To-Hero/dia03-elasticsearch) | [Dia 04](https://techlipe.github.io/Workshop-Zero-To-Hero/dia04-logstash) | [Dia 05](https://techlipe.github.io/Workshop-Zero-To-Hero/dia05-kibana) | 

# Workshop Elastic - Zero to Hero (Dia 3) - Elasticsearch
* **Criado por:** Felipe Queiroz <br>
* **Última atualização:** 04.04.2020

![slide](https://github.com/AnselmoBorges/zerotohero/blob/master/Slide1.jpg)

Fala pessoal! Sejam muito bem vindos ao nosso Dia 04 de Workshop de Zero to Hero com toda a Elastic Stack. Hoje vimos como funciona o Elasticsearch e pudemos entender como que trabalha o coração da Stack, o que são índices, documentos, mapeamentos dentre outros temas que são detalhados nesse documento. Espero que tenha gostado ;) 


# The Heart of the Stack: Elasticsearch
**Observação importante: Para seguir esse tutorial acessar Kibana > Dev Tools ;)**

**O que é um Nó e um Cluster Elasticsearch ?**
Nó é uma instância de Elasticsearch no ar, ou seja, quando incializamos o Elasticsearch (independente da maneira) temos um nó iniciado. Já um cluster também iniciado a partir de um nó, porém, um cluster pode ter múltiplos nós dentro deles, ou seja, um cluster também pode ser um agrupapemtno de nós de diversos papéis.

Se realizarmos uma chamada no contexto '/'
```
GET /
```

Teremos as informações gerais do nosso cluster, como o exemplo abaixo:
```
{
  "name" : "e3617abde627",
  "cluster_name" : "docker-cluster",
  "cluster_uuid" : "JnJggtUFR16lNwstxUfl1g",
  "version" : {
    "number" : "7.6.1",
    "build_flavor" : "default",
    "build_type" : "docker",
    "build_hash" : "aa751e09be0a5072e8570670309b1f12348f023b",
    "build_date" : "2020-02-29T00:15:25.529771Z",
    "build_snapshot" : false,
    "lucene_version" : "8.4.0",
    "minimum_wire_compatibility_version" : "6.8.0",
    "minimum_index_compatibility_version" : "6.0.0-beta1"
  },
  "tagline" : "You Know, for Search"
}
```

**Interfaces HTTP e Transport (TCP)**
O Elasticsearch trabalha com duas camadas de comunicação, uma HTTP REST para atender requisições client-side e outra TCP (Transport) que atende as demandas internas do cluster. Como vimos, a camada HTTP é onde o Kibana consome as informações do Elasticsearch e onde nós trabalharemos no nosso workshop, já a camada de transporte podemos imaginar um seguinte cenário.


![](https://www.websequencediagrams.com/?png=msc866396517)

## Indices
**Definição 1) Mapeamento e Schema-FREE**

**Definição 2) Documentos**

**Configurações de ìndices**

## API's
**_cat/**

**_cluster/health**

**_bulk/**


## Breve Apresentação a Buscas
