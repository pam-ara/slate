---
title: API Reference

language_tabs:
  - python

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='http://github.com/tripit/slate'>Documentation Powered by Slate</a>

search: true
---

# Introdução

Essa é a API LiveCapital. Nela estão descritos todos os recursos disponíves e a forma de acessá-los utitlizando os principais métodos do protocolo HTTP.

#Clientes

##Recursos

Esses são todos os recursos de Clientes disponíveis.

Recurso | Método | Descrição
------- | ------ | ---------
[/clients/menu](#get-clients-menu) | GET | Lista instituições e suas contas
[/accordions/{name}/{year}](#get-accordions-name-year) | GET | Lista
[/accordions/{name}/{year}-{month}](#get-accordions-name-year-month) | GET | Lista
[/operations/{name}/{year}](#get-operations-name-year) | GET | Lista
[/operations/{name}/{year}-{month}](#get-operations-name-year-month) | GET | Lista
[/portfolios/{name}/{year}](#get-portfolios-name-year) | GET | Lista
[/portfolios/{name}/{year}-{month}](#get-portfolios-name-year-month) | GET | Lista
[/returns/{name}/{year}](#get-returns-name-year) | GET | Lista
[/returns/{name}/{year}-{month}](#get-returns-name-year-month) | GET | Lista


##GET /clients/menu

```python
import requests

request = requests.get('http://api.livecapital.com/clients/menu/')

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de todas as instituições e suas contas.

### HTTP Request

`GET http://api.livecapital.com/clients/menu/`

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /accordions/{name}/{year}

```python
import requests

request = request.get(
  'http://api.livecapital.com/clients/accordions/{}/{}/'.format(name, year))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/accordions/{name}/{year}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
name | Nome da instituição
year | Ano no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /accordions/{name}/{year}-{month}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/clients/accordions/{}/{}-{}/'\
  .format(name, year, month)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/accordions/{name}/{year}-{month}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
name | Nome da instituição
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /operations/{name}/{year}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/clients/operations/{}/{}/'.format(name, year))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/operations/{name}/{year}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
name | Nome da instituição
year | Ano no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /operations/{name}/{year}-{month}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/clients/operations/{}/{}-{}/'\
  .format(name, year, month)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/operations/{name}/{year}-{month}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
name | Nome da instituição
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /portfolios/{name}/{year}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/clients/portfolios/{}/{}/'.format(name, year))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/portfolios/{name}/{year}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
name | Nome da instituição
year | Ano no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /portfolios/{name}/{year}-{month}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/clients/portfolios/{}/{}-{}/'\
  .format(name, year, month)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/portfolios/{name}/{year}-{month}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /returns/{name}/{year}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/clients/returns/{}/{}/'.format(name, year))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/returns/{name}/{year}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
name | Nome da instituição
year | Ano no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /returns/{name}/{year}-{month}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/clients/returns/{}/{}-{}/'\
  .format(name, year, month)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/returns/{name}/{year}-{month}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
name | Nome da instituição
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |



#Instituições


## Recursos

Esses são todos os recursos de instituições disponíveis.

Recurso | Método | Descrição
------- | ------ | ---------
[/institutions/official](#get-institutions-official) | GET | Lista todas as instituinções oficiais
[/institutions/official/{id}](#get-institutions-official-id) | GET | Retorna uma instituição oficial específica
[/institutions/custom](#get-institutions-custom) | GET | Lista todas as instituições de um usuário autenticado
[/institutions/custom](#post-institutions-custom) | POST | Cria uma instituição para um usuário
[/institutions/custom/{id}](#get-institutions-custom-id) | GET | Retorna uma determinada instituição de um usuário
[/institutions/custom/{id}](#put-institutions-custom-id) | PUT | Altera dados de uma instituição
[/institutions/custom/{id}](#delete-institutions-custom-id) | DELETE | Apaga uma instituição


##GET /institutions/official

```python
import requests

request = requests.get('http://api.livecapital.com/institutions/official/')

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
[
  {
    "id": 1,
    "name": "HSBC BANK BRASIL S.A. - BANCO MULTIPLO",
    "category": "BROKER"
  },
  {
    "id": 2,
    "name": "BANCO SANTANDER (BRASIL) S.A.",
    "category": "BROKER"
  },
  {
    "id": 3,
    "name": "C.S.MENDES AGENTE AUTÔNOMO DE INVESTIMENTOS LTDA",
    "category": "AUTONOMOUS_AGENT"
  },
  {
    "id": 4,
    "name": "LATOMIA AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
    "category": "AUTONOMOUS_AGENT"
  },
  {
    "id": 5,
    "name": "PREFEITURA DO MUNICÍPIO DE SÃO PAULO",
    "category": "BROKER"
  }
]
```

Esse recurso retorna uma lista com todas as instituições oficiais.

### HTTP Request

`GET http://api.livecapital.com/institutions/official/`

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição
name | Nome da instituição
category | Categoria da institutição. Podendo ser seguradora (BROKER), ou agente autonomo (AUTONOMOUS_AGENT)


##GET /institutions/official/{id}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/institutions/official/{}/'.format(id))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 2,
  "name": "BANCO SANTANDER (BRASIL) S.A.",
  "address": "AV PRESIDENTE JUSC KUBITSCHEK, 2041 E 2235, VL OLIMPIA, SÃO PAULO, SP, 4543011",
  "phone": "(11) 35535533",
  "fax": "(11) 35535533",
  "category": "BROKER",
  "person_type": "LEGAL_PERSON",
  "identifier": "90400888000142",
  "social_denomination": "BANCO SANTANDER (BRASIL) S.A.",
  "commercial_denomination": "BANCO SANTANDER (BRASIL) S.A.",
  "email": "juridsocietario@santander.com.br",
  "zip_code": "4543011",
  "district": "VL OLIMPIA",
  "street": "AV PRESIDENTE JUSC KUBITSCHEK",
  "complement": "2041 E 2235",
  "city": "SÃO PAULO",
  "uf": "SP"
}
```

Esse recurso retorna dados de uma determinada instituição.

### HTTP Request

`GET http://api.livecapital.com/institutions/official/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
id | Id da instituição que será retornada

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição
name | Nome da instituição
address | Endereço da instutição
zip_code | CEP da instituição
district | Distrito da instituição
street | Rua da instituição
complement | Complemento do endereço
city | Cidade da instituição
uf | Código do Estado - Unidade Federativa
phone | Telefone da instituição
fax | Fax da instituição
email | Email da instituição
category | Categoria da institutição. Podendo ser seguradora (BROKER), ou agente autonomo (AUTONOMOUS_AGENT)
person_type | Tipo de pessoa
identifier | Número identificador
social_denomination | Denominação social
commercial_denomination | Denominação comercial


##GET /institutions/custom

```python
import requests

request = requests.get(
  'http://api.livecapital.com/users/{}/institutions/custom/'.format(username))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
[
  {
    "id": 318,
    "broker": {
      "id": 28,
      "name": "HSBC BANK BRASIL S.A. - BANCO MULTIPLO",
      "address": "TRAVESSA OLIVEIRA BELO, Nº 34, 4º ANDAR, CENTRO, CURITIBA, PR, 80020030",
      "phone": "(41) 37775384",
      "fax": "(41) 37775732",
      "category": "BROKER",
      "person_type": "LEGAL_PERSON",
      "identifier": "1701201000189",
      "social_denomination": "HSBC BANK BRASIL S.A. - BANCO MULTIPLO",
      "commercial_denomination": "HSBC BANK BRASIL S.A. - BANCO MULTIPLO",
      "email": "davieira@hsbc.com.br",
      "zip_code": "80020030",
      "district": "CENTRO",
      "street": "TRAVESSA OLIVEIRA BELO, Nº 34",
      "complement": "4º ANDAR",
      "city": "CURITIBA",
      "uf": "PR"
    },
    "autonomous_agent": null,
    "trading_accounts": [],
    "name": "HSBC"
  },
  {
    "id": 319,
    "broker": null,
    "autonomous_agent": {
      "id": 1295,
      "name": "UNITY AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
      "address": "",
      "phone": "",
      "fax": "",
      "category": "AUTONOMOUS_AGENT",
      "person_type": "LEGAL_PERSON",
      "identifier": "7491320000130",
      "social_denomination": "UNITY AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
      "commercial_denomination": "",
      "email": "sandro.marques@prospercorretora.com.br",
      "zip_code": "",
      "district": "",
      "street": "",
      "complement": "",
      "city": "",
      "uf": ""
    },
    "trading_accounts": [],
    "name": "UNITY"
  },
  {
    "id": 320,
    "broker": {
      "id": 1,
      "name": "BANCO SANTANDER (BRASIL) S.A.",
      "address": "AV PRESIDENTE JUSC KUBITSCHEK, 2041 E 2235, VL OLIMPIA, SÃO PAULO, SP, 4543011",
      "phone": "(11) 35535533",
      "fax": "(11) 35535533",
      "category": "BROKER",
      "person_type": "LEGAL_PERSON",
      "identifier": "90400888000142",
      "social_denomination": "BANCO SANTANDER (BRASIL) S.A.",
      "commercial_denomination": "BANCO SANTANDER (BRASIL) S.A.",
      "email": "juridsocietario@santander.com.br",
      "zip_code": "4543011",
      "district": "VL OLIMPIA",
      "street": "AV PRESIDENTE JUSC KUBITSCHEK",
      "complement": "2041 E 2235",
      "city": "SÃO PAULO",
      "uf": "SP"
    },
    "autonomous_agent": {
      "id": 2,
      "name": "LATOMIA AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
      "address": "",
      "phone": "",
      "fax": "",
      "category": "AUTONOMOUS_AGENT",
      "person_type": "LEGAL_PERSON",
      "identifier": "9168994000124",
      "social_denomination": "LATOMIA AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
      "commercial_denomination": "LATOMIA AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
      "email": "latomia@yahoo.com",
      "zip_code": "",
      "district": "",
      "street": "",
      "complement": "",
      "city": "",
      "uf": ""
    },
    "trading_accounts": [],
    "name": "LATOMIA"
  },
  {
    "id": 321,
    "broker": null,
    "autonomous_agent": null,
    "trading_accounts": [],
    "name": "PREFEITURA DO MUNICÍPIO DE SÃO PAULO"
  }
]
```

Este recurso lista todas as instituições de um usuário autenticado.

### HTTP Request

`GET http://api.livecapital.com/users/{username}/institutions/custom/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
username | Nome de um usuário autenticado

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição do usuário
broker | Instituição do tipo "BROKER"
autonomous_agent | Instituição do tipo "AUTONOMOUS_AGENT"
trading_accounts | Contas relacionadas a instituição
name | Nome da instutuição do usuário

### Parâmetros de BROKER/AUTONOMOUS_AGENT

Parâmetro | Descrição
--------- | ---------
id | Id da instituição
name | Nome da instituição
address | Endereço da instutição
zip_code | CEP da instituição
district | Distrito da instituição
street | Rua da instituição
complement | Complemento do endereço
city | Cidade da instituição
uf | Código do Estado - Unidade Federativa
phone | Telefone da instituição
fax | Fax da instituição
email | Email da instituição
category | Categoria da institutição. Podendo ser seguradora (BROKER), ou agente autonomo (AUTONOMOUS_AGENT)
person_type | Tipo de pessoa
identifier | Número identificador
social_denomination | Denominação social
commercial_denomination | Denominação comercial


##POST /institutions/custom

```python
import requests

values = {
          "name": "BANCO SANTANDER (BRASIL) S.A.",
          "broker": 1,
          "autonomous_agent": 2,
          "trading_accounts":[]
        }

request = requests.post(
  'http://api.livecapital.com/users/{}/institutions/custom/'.format(username),
  data=values
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 1,
  "broker": {
    "id": 1,
    "name": "BANCO SANTANDER (BRASIL) S.A.",
    "address": "AV PRESIDENTE JUSC KUBITSCHEK, 2041 E 2235, VL OLIMPIA, SÃO PAULO, SP, 4543011",
    "phone": "(11) 35535533",
    "fax": "(11) 35535533",
    "category": "BROKER",
    "person_type": "LEGAL_PERSON",
    "identifier": "90400888000142",
    "social_denomination": "BANCO SANTANDER (BRASIL) S.A.",
    "commercial_denomination": "BANCO SANTANDER (BRASIL) S.A.",
    "email": "juridsocietario@santander.com.br",
    "zip_code": "4543011",
    "district": "VL OLIMPIA",
    "street": "AV PRESIDENTE JUSC KUBITSCHEK",
    "complement": "2041 E 2235",
    "city": "SÃO PAULO",
    "uf": "SP"
  },
  "autonomous_agent": {
    "id": 2,
    "name": "LATOMIA AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
    "address": "",
    "phone": "",
    "fax": "",
    "category": "AUTONOMOUS_AGENT",
    "person_type": "LEGAL_PERSON",
    "identifier": "9168994000124",
    "social_denomination": "LATOMIA AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
    "commercial_denomination": "LATOMIA AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
    "email": "latomia@yahoo.com",
    "zip_code": "",
    "district": "",
    "street": "",
    "complement": "",
    "city": "",
    "uf": ""
  },
  "trading_accounts": [],
  "name": "BANCO SANTANDER (BRASIL) S.A."
}
```

Este recurso cria uma instituição para um determinado usuário autenticado.

### HTTP Request

`POST http://api.livecapital.com/users/{username}/institutions/custom/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
username | Nome de um usuário autenticado

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição do usuário
broker | Instutição do tipo BROKER
autonomous_agent | Instutição do tipo "AUTONOMOUS_AGENT
trading_accounts | Contas relacioandas a instituição
name | Nome da instutuição do usuário

### Parâmetros de BROKER/AUTONOMOUS_AGENT

Parâmetro | Descrição
--------- | ---------
id | Id da instituição
name | Nome da instituição
address | Endereço da instutição
zip_code | CEP da instituição
district | Distrito da instituição
street | Rua da instituição
complement | Complemento do endereço
city | Cidade da instituição
uf | Código do Estado - Unidade Federativa
phone | Telefone da instituição
fax | Fax da instituição
email | Email da instituição
category | Categoria da institutição. Podendo ser seguradora (BROKER), ou agente autonomo (AUTONOMOUS_AGENT)
person_type | Tipo de pessoa
identifier | Número identificador
social_denomination | Denominação social
commercial_denomination | Denominação comercial


##GET /institutions/custom/{id}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/users/{}/institutions/custom/{}/'\
  .format(username, id)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 1,
  "broker": {
    "id": 1,
    "name": "BANCO SANTANDER (BRASIL) S.A.",
    "address": "AV PRESIDENTE JUSC KUBITSCHEK, 2041 E 2235, VL OLIMPIA, SÃO PAULO, SP, 4543011",
    "phone": "(11) 35535533",
    "fax": "(11) 35535533",
    "category": "BROKER",
    "person_type": "LEGAL_PERSON",
    "identifier": "90400888000142",
    "social_denomination": "BANCO SANTANDER (BRASIL) S.A.",
    "commercial_denomination": "BANCO SANTANDER (BRASIL) S.A.",
    "email": "juridsocietario@santander.com.br",
    "zip_code": "4543011",
    "district": "VL OLIMPIA",
    "street": "AV PRESIDENTE JUSC KUBITSCHEK",
    "complement": "2041 E 2235",
    "city": "SÃO PAULO",
    "uf": "SP"
  },
  "autonomous_agent": {
    "id": 2,
    "name": "LATOMIA AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
    "address": "",
    "phone": "",
    "fax": "",
    "category": "AUTONOMOUS_AGENT",
    "person_type": "LEGAL_PERSON",
    "identifier": "9168994000124",
    "social_denomination": "LATOMIA AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
    "commercial_denomination": "LATOMIA AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
    "email": "latomia@yahoo.com",
    "zip_code": "",
    "district": "",
    "street": "",
    "complement": "",
    "city": "",
    "uf": ""
  },
  "trading_accounts": [],
  "name": "BANCO SANTANDER (BRASIL) S.A."
}
```

Este recurso retorna uma determinada instituição de um usuário autenticado.

### HTTP Request

`GET http://api.livecapital.com/users/{username}/institutions/custom/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
username | Nome de um usuário autenticado
id | Id de uma instituição de usuário

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição do usuário
broker | Institutição do tipo BROKER
autonomous_agent | Institutição do tipo AUTONOMOUS_AGENT
trading_accounts | Contas relacionadas a instituição
name | Nome da instutuição do usuário

### Parâmetros de BROKER/AUTONOMOUS_AGENT

Parâmetro | Descrição
--------- | ---------
id | Id da instituição
name | Nome da instituição
address | Endereço da instutição
zip_code | CEP da instituição
district | Distrito da instituição
street | Rua da instituição
complement | Complemento do endereço
city | Cidade da instituição
uf | Código do Estado - Unidade Federativa
phone | Telefone da instituição
fax | Fax da instituição
email | Email da instituição
category | Categoria da institutição. Podendo ser seguradora (BROKER), ou agente autonomo (AUTONOMOUS_AGENT)
person_type | Tipo de pessoa
identifier | Número identificador
social_denomination | Denominação social
commercial_denomination | Denominação comercial


##PUT /institutions/custom/{id}

```python
import requests

values = {
          "name": "HSBC BANK BRASIL S.A.",
          "broker": 28,
          "autonomous_agent": 1295,
          "trading_accounts": [],
        }

request = requests.put(
  'http://api.livecapital.com/institutions/custom/{}/'.format(id), json=values)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 1,
  "broker": {
    "id": 28,
    "name": "HSBC BANK BRASIL S.A. - BANCO MULTIPLO",
    "address": "TRAVESSA OLIVEIRA BELO, Nº 34, 4º ANDAR, CENTRO, CURITIBA, PR, 80020030",
    "phone": "(41) 37775384",
    "fax": "(41) 37775732",
    "category": "BROKER",
    "person_type": "LEGAL_PERSON",
    "identifier": "1701201000189",
    "social_denomination": "HSBC BANK BRASIL S.A. - BANCO MULTIPLO",
    "commercial_denomination": "HSBC BANK BRASIL S.A. - BANCO MULTIPLO",
    "email": "davieira@hsbc.com.br",
    "zip_code": "80020030",
    "district": "CENTRO",
    "street": "TRAVESSA OLIVEIRA BELO, Nº 34",
    "complement": "4º ANDAR",
    "city": "CURITIBA",
    "uf": "PR"
  },
  "autonomous_agent": {
    "id": 1295,
    "name": "UNITY AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
    "address": "",
    "phone": "",
    "fax": "",
    "category": "AUTONOMOUS_AGENT",
    "person_type": "LEGAL_PERSON",
    "identifier": "7491320000130",
    "social_denomination": "UNITY AGENTES AUTONOMOS DE INVESTIMENTOS LTDA",
    "commercial_denomination": "",
    "email": "sandro.marques@prospercorretora.com.br",
    "zip_code": "",
    "district": "",
    "street": "",
    "complement": "",
    "city": "",
    "uf": ""
  },
  "trading_accounts": [],
  "name": "HSBC BANK BRASIL S.A."
}
```

Este recurso altera uma determinada instituição de um usuário autenticado.

### HTTP Request

`PUT http://api.livecapital.com/users/{username}/institutions/custom/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
username | Nome de um usuário autenticado
id | Id de uma instituição de usuário

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição do usuário
broker | Institutição do tipo BROKER
autonomous_agent | Institutição do tipo AUTONOMOUS_AGENT
trading_accounts | Contas relacionadas a instituição
name | Nome da instutuição do usuário

### Parâmetros de BROKER/AUTONOMOUS_AGENT

Parâmetro | Descrição
--------- | ---------
id | Id da instituição
name | Nome da instituição
address | Endereço da instutição
zip_code | CEP da instituição
district | Distrito da instituição
street | Rua da instituição
complement | Complemento do endereço
city | Cidade da instituição
uf | Código do Estado - Unidade Federativa
phone | Telefone da instituição
fax | Fax da instituição
email | Email da instituição
category | Categoria da institutição. Podendo ser seguradora (BROKER), ou agente autonomo (AUTONOMOUS_AGENT)
person_type | Tipo de pessoa
identifier | Número identificador
social_denomination | Denominação social
commercial_denomination | Denominação comercial


##DELETE /institutions/custom/{id}

```python
import requests

request = requests.delete(
  'http://api.livecapital.com/users/{}/institutions/custom/{}/'\
  .format(username, id)
)
```

Este recurso apaga uma determinada instituição de um usuário autenticado.

### HTTP Request

`DELETE http://api.livecapital.com/users/{username}/institutions/custom/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
username | Nome de um usuário autenticado
id | Id de uma instituição de usuário

#DARF

## Recursos

Esses são todos os recursos de DARF disponíveis.

Recurso | Método | Descrição
------- | ------ | ---------
[/darf/{year}-{month}/reports](#get-year-month-reports) | GET |  Exibe o relatório
[/darf/{year}-{month}/print](#get-year-month-print) | GET | Exibe DARF

##GET /{year}-{month}/reports

```python
import requests

request = requests.get(
  'http://api.livecapital.com/darf/{}-{}/reports/'.format(year, month))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso exibe um relatório filtrado por mês e ano.

### HTTP Request

`GET http://api.livecapital.com/darf/{year}-{month}/reports/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /{year}-{month}/print

```python
import requests

request = requests.get(
  'http://api.livecapital.com/darf/{}-{}/print/'.format(year, month))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso exibe uma DARF filtrada por mês e ano.

### HTTP Request

`GET http://api.livecapital.com/darf/{year}-{month}/print/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |



#Bovespa


##Recursos

Esses são todos os recursos de Bovespa disponíveis.

Recurso | Método | Descrição
------- | ------ | ---------
[/bovespa/{custom-institution}/trading-accounts](#get-bovespa-custom-institution-trading-accounts) | GET | Lista todas as contas de Bovespa de uma determinada instituição de um usuário autenticado
[/bovespa/{custom-institution}/trading-accounts](#post-bovespa-custom-institution-trading-accounts) | POST | Cria uma conta de Bovespa para uma instituição de um usuário autenticado
[/bovespa/{custom-institution}/trading-accounts/{id}](#get-bovespa-custom-institution-trading-accounts-id) | GET | Exibe os dados de uma conta Bovespa
[/bovespa/{custom-institution}/trading-accounts/{id}](#put-bovespa-custom-institution-trading-accounts-id) | PUT | Altera os dados de uma conta Bovespa
[/bovespa/{custom-institution}/trading-accounts/{id}](#delete-bovespa-custom-institution-trading-accounts-id) | DELETE | Apaga uma conta Bovespa
[/bovespa/assets](#get-bovespa-assets) | GET | Retorna uma lista de ativos
[/bovespa/brokerage-notes](#post-bovespa-brokerage-notes) | POST | Cria uma nota de corretagem
[/bovespa/brokerage-notes/{id}](#get-bovespa-brokerage-notes-id) | GET | Exibe dados da nota de corretagem
[/bovespa/brokerage-notes/{id}](#put-bovespa-brokerage-notes-id) | PUT | Altera dados da nota de corretagem
[/bovespa/brokerage-notes/{id}](#delete-bovespa-brokerage-notes-id) | DELETE | Apaga uma nota de corretagem
[/bovespa/positions/{date}/terms](#get-bovespa-positions-date-terms) | GET | Retorna a posição da conta na data informada apenas por termos
[/bovespa/positions/{date}/non-terms](#get-bovespa-positions-date-non-terms) | GET | Retorna a posição da conta na data informada sem termos
[/bovespa/events/{trading-account}/{date}](#get-bovespa-events-trading-account-date) | GET | Lista todos os eventos de uma conta filtrados por data
[/bovespa/{event-type}/{id}](#get-bovespa-event-type-id) | GET | Exibe dados de um evento
[/bovespa/{event-type}/{id}](#put-bovespa-event-type-id) | PUT | Altera dados de um evento
[/bovespa/{event-type}/{id}](#delete-bovespa-event-type-id) | DELETE | Apaga um evento


##GET /bovespa/{custom-institution}/trading-accounts

```python
import requests

request = requests.get(
  'http://api.livecapital.com/bovespa/{}/trading-accounts/'.format(custom_institution))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
[
  {
    "id": 1,
    "account_type": "STOCK",
    "linked_account_identifier": "04678321",
    "linked_account_name": "HSBC",
    "identifier": "17263580",
    "name": "Bovespa",
    "linked_account": 4
  },
  {
    "id": 2,
    "account_type": "STOCK",
    "linked_account_identifier": null,
    "linked_account_name": null,
    "identifier": "00385230",
    "name": "Bov",
    "linked_account": null
  },
  {
    "id": 3,
    "account_type": "STOCK",
    "linked_account_identifier": "00573283",
    "linked_account_name": "Itau",
    "identifier": "05830151",
    "name": "Global bovespa",
    "linked_account": 40
  }
]
```

Esse recurso lista todas as contas de Bovespa de uma instituição de um usuário autenticado.

### HTTP Request

`GET http://api.livecapital.com/bovespa/{custom-institution}/trading-accounts/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta de Bovespa
account_type | Tipo da conta. Será sempre Bovespa(STOCK), pois não pode ser alterado
linked_account_identifier | Número identificador de uma conta corrente associada
linked_account_name | Nome de uma conta corrente associada
identifier | Número identificador da conta
name | Nome da conta
linked_account | Id da uma conta corrente associada


##POST /bovespa/{custom-institution}/trading-accounts

```python
import requests

values = {
  "name": "Bovespa",
  "identifier": "09343260",
  "linked_account": 4
}

request = requests.post(
  'http://api.livecapital.com/bovespa/{}/trading-accounts/'.format(custom_institution),
  json=values
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 6,
  "account_type": "STOCK",
  "linked_account_identifier": "04678321",
  "linked_account_name": "HSBC",
  "identifier": "09343260",
  "name": "Bovespa",
  "linked_account": 4
}
```

Esse recurso cria uma conta Bovespa para uma instituição de um usuário autenticado.

### HTTP Request

`POST http://api.livecapital.com/bovespa/{custom-institution}/trading-accounts/`

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta de Bovespa
account_type | Tipo da conta. Será sempre Bovespa(STOCK), pois não pode ser alterado
linked_account_identifier | Número identificador de uma conta corrente associada
linked_account_name | Nome de uma conta corrente associada
identifier | Número identificador da conta
name | Nome da conta
linked_account | Id da uma conta corrente associada


##GET /bovespa/{custom-institution}/trading-accounts/{id}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/bovespa/{}/trading-accounts/{}/'\
  .format(custom_institution, id)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 6,
  "account_type": "STOCK",
  "linked_account_identifier": "04678321",
  "linked_account_name": "HSBC",
  "identifier": "09343260",
  "name": "Bovespa",
  "linked_account": 4
}
```

Esse recurso retorna dados de uma determinada conta bovespa.

### HTTP Request

`GET http://api.livecapital.com/bovespa/{custom-institution}/trading-accounts/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado
id | Id de uma conta

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta de Bovespa
account_type | Tipo da conta. Será sempre Bovespa(STOCK), pois não pode ser alterado
linked_account_identifier | Número identificador de uma conta corrente associada
linked_account_name | Nome de uma conta corrente associada
identifier | Número identificador da conta
name | Nome da conta
linked_account | Id da uma conta corrente associada


##PUT /bovespa/{custom-institution}/trading-accounts/{id}

```python
import requests

values = {
          "name": "Global Bov",
          "identifier": "00347501",
          "linked_account": 40
        }

request = requests.put('http://api.livecapital.com/bovespa/{}/trading-accounts/{}/'\
  .format(custom_institution, id), json=values)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 8,
  "account_type": "STOCK",
  "linked_account_identifier": "00573283",
  "linked_account_name": "Itau",
  "identifier": "00347501",
  "name": "Global Bov",
  "linked_account": 40
}
```

Esse recurso altera dados de uma determinada conta bovespa.

### HTTP Request

`PUT http://api.livecapital.com/bovespa/{custom-institution}/trading-accounts/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado
id | Id de uma conta

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta de Bovespa
account_type | Tipo da conta. Será sempre Bovespa(STOCK), pois não pode ser alterado
linked_account_identifier | Número identificador de uma conta corrente associada
linked_account_name | Nome de uma conta corrente associada
identifier | Número identificador da conta
name | Nome da conta
linked_account | Id da uma conta corrente associada


##DELETE /bovespa/{custom-institution}/trading-accounts/{id}

```python
import requests

request = requests.delete('http://api.livecapital.com/bovespa/{}/trading-accounts/{}/'\
  .format(custom_institution, id))

request.json()
```

Este recurso apaga uma determinada conta bovespa.

### HTTP Request

`DELETE http://api.livecapital.com/bovespa/{custom-institution}/trading-accounts/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado
id | Id de uma conta bovespa


##GET /bovespa/assets

```python
import requests

request = requests.get('http://api.livecapital.com/bovespa/assets/')

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de ativos.

### HTTP Request

`GET http://api.livecapital.com/bovespa/assets/`

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##POST /bovespa/brokerage-notes

```python
import requests

values = {}

request = requests.post(
  'http://api.livecapital.com/bovespa/brokerage-notes/', data=values)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso cria uma nota de corretagem.

### HTTP Request

`POST http://api.livecapital.com/bovespa/brokerage-notes/`

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /bovespa/brokerage-notes/{id}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/bovespa/brokerage-notes/{}/'.format(id))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna os dados de uma nota de corretagem.

### HTTP Request

`GET http://api.livecapital.com/bovespa/brokerage-notes/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
id | Id da nota de corretagem

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##PUT /bovespa/brokerage-notes/{id}

```python
import requests

values = {}

request = requests.put(
  'http://api.livecapital.com/bovespa/brokerage-notes/{}/'.format(id),
  json=values
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso altera dados de uma nota de corretagem.

### HTTP Request

`PUT http://api.livecapital.com/bovespa/brokerage-notes/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
id | Id da nota de corretagem

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##DELETE /bovespa/brokerage-notes/{id}

```python
import requests

request = requests.delete(
  'http://api.livecapital.com/bovespa/brokerege-notes/{}/'.format(id))
```

Esse recurso apaga uma nota de corretagem.

### HTTP Request

`DELETE http://api.livecapital.com/bovespa/brokerage-notes/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
id | Id da nota de corretagem

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /bovespa/positions/{date}/terms

```python
import requests

request = requests.get(
  'http://api.livecapital.com/bovespa/positions/{}/terms/'.format(date))

request.json
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna a posição da conta na data informada exibindo apenas os termos.

### HTTP Request

`GET http://api.livecapital.com/bovespa/positions/{date}/terms/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
date | Data na qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /bovespa/positions/{date}/non-terms

```python
import requests

request = requests.get(
  'http://api.livecapital.com/bovespa/positions/{}/non-terms/'.format(date))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna a posição da conta na data informada, mas não exibe os termos.

### HTTP Request

`GET http://api.livecapital.com/bovespa/positions/{date}/non-terms/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
date | Data na qual deseja realizar o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /bovespa/events/{trading-account}/{date}

```python
import requests

request = requests.get('http://api.livecapital.com/bovespa/events/{}/{}/'\
  .format(trading-account, date)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso lista todos os eventos de uma conta filtrando por data.

### HTTP Request

`GET http://api.livecapital.com/bovespa/events/{trading-account}/{date}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
date | Data na qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /bovespa/{event-type}/{id}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/bovespa/{}/{}/'.format(event-type, id))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna dados de um evento.

### HTTP Request

`GET http://api.livecapital.com/bovespa/{event-type}/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
event-type | Tipo de evento que se deseja consultar.
id | Id do evento

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##PUT /bovespa/{event-type}/{id}

```python
import requests

values = {}

request = requests.put('http://api.livecapital.com/bovespa/{}/{}/'\
  .format(event-type, id), json=values
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso altera dados de um evento.

### HTTP Request

`PUT http://api.livecapital.com/bovespa/{event-type}/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
event-type | Tipo de evento que se deseja consultar.
id | Id do evento

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##DELETE /bovespa/{event-type}/{id}

```python
import requests

request = requests.delete(
  'http://api.livecapital.com/bovespa/{}/{}/'.format(event_type, id))
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso apaga um evento.

### HTTP Request

`DELETE http://api.livecapital.com/bovespa/{event-type}/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
event-type | Tipo de evento que se deseja consultar.
id | Id do evento

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |



#BTC

##Recursos

Esses são todos os recursos de BTC disponíveis.

Recurso | Método | Descrição
------- | ------ | ---------
[/btc/{custom-institution}/trading-accounts](#get-btc-custom-institution-trading-accounts) | GET | Lista todas as contas de BTC de uma determinada instituição de um usuário autenticado
[/btc/{custom-institution}/trading-accounts](#post-btc-custom-institution-trading-accounts) | POST | Cria uma conta de BTC para uma instituição de um usuário autenticado
[/btc/{custom-institution}/trading-accounts/{id}](#get-btc-custom-institution-trading-accounts-id) | GET | Exibe os dados de uma conta BTC
[/btc/{custom-institution}/trading-accounts/{id}](#put-btc-custom-institution-trading-accounts-id) | PUT | Altera os dados de uma conta BTC
[/btc/{custom-institution}/trading-accounts/{id}](#delete-btc-custom-institution-trading-accounts-id) | DELETE | Apaga uma conta BTC


##GET /btc/{custom-institution}/trading-accounts

```python
import requests

request = requests.get(
  'http://api.livecapital.com/btc/{}/trading-accounts/'.format(custom_institution))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
[
  {
    "id": 10,
    "account_type": "BTC",
    "linked_account_identifier": "17263580",
    "linked_account_name": "Bovespa",
    "identifier": "17263580",
    "name": "Btc",
    "linked_account": 1
  },
  {
    "id": 4,
    "account_type": "BTC",
    "linked_account_identifier": null,
    "linked_account_name": null,
    "identifier": "00762301",
    "name": "Nova btc",
    "linked_account": null
  },
  {
    "id": 3,
    "account_type": "BTC",
    "linked_account_identifier": "05830151",
    "linked_account_name": "Global bovespa",
    "identifier": "08845900",
    "name": "Global btc",
    "linked_account": 3
  }
]
```

Esse recurso lista todas as contas de BTC de uma instituição de um usuário autenticado.

### HTTP Request

`GET http://api.livecapital.com/btc/{custom-institution}/trading-accounts/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta de BTC
account_type | Tipo da conta. Será sempre BTC, pois não pode ser alterado
linked_account_identifier | Número identificador de uma conta bovespa associada
linked_account_name | Nome de uma conta bovespa associada
identifier | Número identificador da conta
name | Nome da conta
linked_account | Id da uma conta bovespa associada


##POST /btc/{custom-institution}/trading-accounts

```python
import requests

values = {
  "name": "Btc",
  "identifier": "17263580",
  "linked_account": 1
}

request = requests.post(
  'http://api.livecapital.com/btc/{}/trading-accounts/'.format(custom_institution),
  json=values
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 10,
  "account_type": "BTC",
  "linked_account_identifier": "17263580",
  "linked_account_name": "Bovespa",
  "identifier": "17263580",
  "name": "Btc",
  "linked_account": 1
}
```

Esse recurso cria uma conta BTC para uma instituição de um usuário autenticado.

### HTTP Request

`POST http://api.livecapital.com/btc/{custom-institution}/trading-accounts/`

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta de BTC
account_type | Tipo da conta. Será sempre BTC, pois não pode ser alterado
linked_account_identifier | Número identificador de uma conta bovespa associada
linked_account_name | Nome de uma conta bovespa associada
identifier | Número identificador da conta
name | Nome da conta
linked_account | Id da uma conta bovespa associada


##GET /btc/{custom-institution}/trading-accounts/{id}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/btc/{}/trading-accounts/{}/'\
  .format(custom_institution, id)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 10,
  "account_type": "BTC",
  "linked_account_identifier": "17263580",
  "linked_account_name": "Bovespa",
  "identifier": "17263580",
  "name": "Btc",
  "linked_account": 1
}
```

Esse recurso retorna dados de uma determinada conta btc.

### HTTP Request

`GET http://api.livecapital.com/btc/{custom-institution}/trading-accounts/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado
id | Id de uma conta

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta de BTC
account_type | Tipo da conta. Será sempre BTC, pois não pode ser alterado
linked_account_identifier | Número identificador de uma conta bovespa associada
linked_account_name | Nome de uma conta bovespa associada
identifier | Número identificador da conta
name | Nome da conta
linked_account | Id da uma conta bovespa associada


##PUT /btc/{custom-institution}/trading-accounts/{id}

```python
import requests

values = {
          "name": "Global btc",
          "identifier": "12398500",
          "linked_account": 3
        }

request = requests.put('http://api.livecapital.com/btc/{}/trading-accounts/{id}/'\
  .format(custom_institution), json=values)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 10,
  "account_type": "BTC",
  "linked_account_identifier": "00573283",
  "linked_account_name": "Itau",
  "identifier": "12398500",
  "name": "Global btc",
  "linked_account": 3
}
```

Esse recurso retorna dados de uma determinada conta btc.

### HTTP Request

`PUT http://api.livecapital.com/btc/{custom-institution}/trading-accounts/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado
id | Id de uma conta

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta de BTC
account_type | Tipo da conta. Será sempre BTC, pois não pode ser alterado
linked_account_identifier | Número identificador de uma conta bovespa associada
linked_account_name | Nome de uma conta bovespa associada
identifier | Número identificador da conta
name | Nome da conta
linked_account | Id da uma conta bovespa associada


##DELETE /btc/{custom-institution}/trading-accounts/{id}

```python
import requests

request = requests.delete('http://api.livecapital.com/btc/{}/trading-accounts/{}/'\
  .format(custom_institution, id))

request.json()
```

Este recurso apaga uma determinada conta btc.

### HTTP Request

`DELETE http://api.livecapital.com/btc/{custom-institution}/trading-accounts/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado
id | Id de uma conta bovespa



#Conta Corrente

##Recursos

Esses são todos os recursos de BTC disponíveis.

Recurso | Método | Descrição
------- | ------ | ---------
[/checking-account/{custom-institution}/trading-accounts](#get-checking-account-custom-institution-trading-accounts) | GET | Lista todas as contas correntes de uma determinada instituição de um usuário autenticado
[/checking-account/{custom-institution}/trading-accounts](#post-checking-account-custom-institution-trading-accounts) | POST | Cria uma conta corrente para uma instituição de um usuário autenticado
[/checking-account/{custom-institution}/trading-accounts/{id}](#get-checking-account-custom-institution-trading-accounts-id) | GET | Exibe os dados de uma conta corrente
[/checking-account/{custom-institution}/trading-accounts/{id}](#put-checking-account-custom-institution-trading-accounts-id) | PUT | Altera os dados de uma conta corrente
[/checking-account/{custom-institution}/trading-accounts/{id}](#delete-checking-account-custom-institution-trading-accounts-id) | DELETE | Apaga uma conta corrente


##GET /checking-account/{custom-institution}/trading-accounts

```python
import requests

request = requests.get(
  'http://api.livecapital.com/checking-account/{}/trading-accounts/'.format(custom_institution))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
[
  {
    "id": 40,
    "account_type": "CHECKING_ACCOUNT",
    "identifier": "00573283",
    "name": "Itau"
  },
  {
    "id": 4,
    "account_type": "CHECKING_ACCOUNT",
    "identifier": "04678321",
    "name": "HSBC"
  },
  {
    "id": 3,
    "account_type": "CHECKING_ACCOUNT",
    "identifier": "17643301",
    "name": "Bradesco"
  }
]
```

Esse recurso lista todas as contas corrente de uma instituição de um usuário autenticado.

### HTTP Request

`GET http://api.livecapital.com/checking-account/{custom-institution}/trading-accounts/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta corrente
account_type | Tipo da conta. Será sempre conta corrente(CHECKING_ACCOUNT), pois não pode ser alterado
identifier | Número identificador da conta
name | Nome da conta


##POST /checking-account/{custom-institution}/trading-accounts

```python
import requests

values = {
  "name": "Santander",
  "identifier": "00345234"
}

request = requests.post(
  'http://api.livecapital.com/checking-account/{}/trading-accounts/'\
  .format(custom_institution), json=values)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 7,
  "account_type": "CHECKING_ACCOUNT",
  "identifier": "00345234",
  "name": "Santander"
}
```

Esse recurso cria uma conta corrente para uma instituição de um usuário autenticado.

### HTTP Request

`POST http://api.livecapital.com/checking-account/{custom-institution}/trading-accounts/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta corrente
account_type | Tipo da conta. Será sempre conta corrente(CHECKING_ACCOUNT), pois não pode ser alterado
identifier | Número identificador da conta
name | Nome da conta


##GET /checking-account/{custom-institution}/trading-accounts/{id}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/checking-account/{}/trading-accounts/{}/'\
  .format(custom_institution, id))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 7,
  "account_type": "CHECKING_ACCOUNT",
  "identifier": "00345234",
  "name": "Santander"
}
```

Esse recurso retorna dados de uma conta corrente.

### HTTP Request

`GET http://api.livecapital.com/checking-account/{custom-institution}/trading-accounts/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado
id | Id de uma conta

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta corrente
account_type | Tipo da conta. Será sempre conta corrente(CHECKING_ACCOUNT), pois não pode ser alterado
identifier | Número identificador da conta
name | Nome da conta


##PUT /checking-account/{custom-institution}/trading-accounts/{id}

```python
import requests

values = {
  "name": "Safra",
  "identifier": "00873451"
}

request = requests.put(
  'http://api.livecapital.com/checking-account/{}/trading-accounts/{}/'\
  .format(custom_institution, id), json=values)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 7,
  "account_type": "CHECKING_ACCOUNT",
  "identifier": "00873451",
  "name": "Safra"
}
```

Esse recurso altera dados de uma conta corrente.

### HTTP Request

`PUT http://api.livecapital.com/checking-account/{custom-institution}/trading-accounts/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado
id | Id de uma conta

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da conta corrente
account_type | Tipo da conta. Será sempre conta corrente(CHECKING_ACCOUNT), pois não pode ser alterado
identifier | Número identificador da conta
name | Nome da conta


##DELETE /checking-account/{custom-institution}/trading-accounts/{id}

```python
import requests

request = requests.delete('http://api.livecapital.com/checking-account/{}/trading-accounts/{}/'\
  .format(custom_institution, id))

request.json()
```

Este recurso apaga uma determinada conta corrente.

### HTTP Request

`DELETE http://api.livecapital.com/checking-account/{custom-institution}/trading-accounts/{id}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
custom-institution | Id de uma instituição de um usuário autenticado
id | Id de uma conta corrente



#Widgets

##Recursos

Esses são todos os recursos de widgets disponíveis.

Recurso | Método | Descrição
------- | ------ | ---------
[/widgets/{name}/{market}/{year}](#get-name-market-year) | GET | Retorna uma lista de widgets filtrados por um ano
[/widgets/{name}/{market}/{year}-{month}](#get-name-market-year-month) | GET | Retorna uma lista de widgets filtrados por um mês e ano
[/widgets/{name}/{market}/{year}-{month}-{day}](#get-name-market-year-month-day) | GET | Retorna uma lista de widgets filtrados por uma data
[/widgets/portfolios/{year}](#get-portfolios-year) | GET | Retorna uma lista de widgets portfolios filtrados por ano
[/widgets/portfolios/{year}-{month}](#get-portfolios-year-month) | GET | Retorna uma lista de widgets portfolios filtrados por mês e ano
[/widgets/portfolios/{year}-{month}-{day}](#get-portfolios-year-month-day) | GET | Retorna uma lista de widgets portfolios filtrados por uma data
[/widgets/capital-gain/{year}](#get-capital-gain-year) | GET | Retorna uma lista de widgets capital-gain filtrados por um ano
[/widgets/capital-gain/{year}-{month}](#get-capital-gain-year-month) | GET | Retorna uma lista de widgets capital-gain filtrados por um mês e ano
[/widgets/capital-gain/{year}-{month}-{day}](#get-capital-gain-year-month-day) | GET | Retorna uma lista de widgets capital-gain filtrados por uma data
[/widgets/taxes/{year}](#get-taxes-year) | GET | Retorna uma lista de widgets taxes filtrados por um ano
[/widgets/taxes/{year}-{month}](#get-taxes-year-month) | GET | Retorna uma lista de widgets taxes filtrados por um mês e ano
[/widgets/taxes/{year}-{month}-{day}](#get-taxes-year-month-day) | GET | Retorna uma lista de widgets taxes filtrados por uma data


##GET /{name}/{market}/{year}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/widgets/{}/{}/{}/'.format(name, market, year))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets de determinado nome filtrados por um ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/{name}/{market}/{year}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
name | Nome do widget
market | Tipo de mercado (Bovespa, BMF, etc)
year | Ano no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /{name}/{market}/{year}-{month}

```python
import requests

request = requests.get('http://api.livecapital.com/widgets/{}/{}/{}-{}/'\
  .format(name, market, year, month)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets de determinado nome filtrados por mês e ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/{name}/{market}/{year}-{month}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
name | Nome do widget
market | Tipo de mercado (Bovespa, BMF, etc)
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /{name}/{market}/{year}-{month}-{day}

```python
import requests

request = requests.get('http://api.livecapital.com/widgets/{}/{}/{}-{}-{}/'\
  .format(name, market, year, month, day)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets de determinado nome filtrados por uma data.

### HTTP Request

`GET http://api.livecapital.com/widgets/{name}/{market}/{year}-{month}-{day}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
name | Nome do widget
market | Tipo de mercado (Bovespa, BMF, etc)
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro
day | Dia no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /portfolios/{year}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/widgets/portfolios/{}/'.format(year))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets portfolio filtrados por um ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/portfolios/{year}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /portfolios/{year}-{month}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/widgets/portfolios/{}-{}/'.format(year, month))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets portfolio filtrados por um mês e ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/portfolios/{year}-{month}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /portfolios/{year}-{month}-{day}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/portfolios/{}-{}-{}/'.format(year, month, day))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets portfolio filtrados por uma data.

### HTTP Request

`GET http://api.livecapital.com/widgets/portfolios/{year}-{month}-{day}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro
day | Dia no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /capital-gain/{year}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/widgets/capital-gain/{}/'.format(year))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets capital-gain filtrados por um ano.

### HTTP Request

`GET http://api.livecapital.com/wigets/capital-gain/{year}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /capital-gain/{year}-{month}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/widgets/capital-gain/{}-{}/'.format(year, month))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets capital-gain filtrados por um mês e ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/capital-gain/{year}-{month}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /capital-gain/{year}-{month}-{day}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/widgets/capital-gain/{}-{}-{}/'\
  .format(year, month, day)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets capital-gain filtrados por uma data.

### HTTP Request

`GET http://api.livecapital.com/widgets/capital-gain/{year}-{month}-{day}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro
day | Dia no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /taxes/{year}

```python
import requests

request = requests(
  'http://api.livecapital.com/widgets/taxes/{}/'.format(year))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets taxes filtrados por um ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/taxes/{year}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /taxes/{year}-{month}

```python
import requests

request = requests.get(
  'http://api.livecapital.com/widgets/taxes/{}-{}/'.format(year, month))

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets taxes filtrados por um mês e ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/taxes/{year}-{month}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |


##GET /taxes/{year}-{month}-{day}

```python
import requests

request = requests.get('http://api.livecapital.com/widgets/taxes/{}-{}-{}/'\
  .format(year, month, day)
)

request.json()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets taxes filtrados por uma data.

### HTTP Request

`GET http://api.livecapital.com/widgets/taxes/{year}-{month}-{day}/`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
year | Ano no qual deseja fazer o filtro
month | Mês no qual deseja fazer o filtro
day | Dia no qual deseja fazer o filtro

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |
