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

#Instituições

## Recursos

Esses são todos os recursos de instituições disponíveis.

Recurso | Método | Descrição
------- | ------ | ---------
/institutions/official | GET | Lista todas as instituinções oficiais
/institutions/official/{id} | GET | Retorna uma instituição oficial específica
/institutions/custom | GET | Lista todas as instituições de um usuário autenticado
/institutions/custom | POST | Cria uma instituição para um usuário
/institutions/custom/{id} | GET | Retorna uma determinada instituição de um usuário
/institutions/custom/{id} | PUT | Atualiza/Altera dados de uma instituição
/institutions/custom/{id} | DELETE | Apaga uma instituição


##GET /official

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/institutions/official')
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição ira retornar um JSON como este:

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

Esse recurso retorna uma lista de todas as instituições oficiais.

### HTTP Request

`GET http://api.livecapital.com/institutions/official`

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição
name | Nome da instituição
category | Tipo de instituição. Existem apenas as categorias "BROKER" e "AUTONOMOUS_AGENT".

##GET /official/{id}

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/institutions/official/{}'.format(id))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição ira retornar um JSON como este:

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
  "uf": "SP",
  "ddd": "11"
}
```

Esse recurso retorna a instituição que tenha o id passado na URL.

### HTTP Request

`GET http://api.livecapital.com/institutions/official/{id}`

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
ddd | DDD da institutição
phone | Telefone da instituição
fax | Fax da instituição
email | Email da instituição
category | Categoria a qual a instituição pertence
person_type | Tipo de pessoa
identifier | Número identificador
social_denomination | Denominação social
commercial_denomination | Denominação comercial

##GET /custom

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/users/{username}institutions/custom')
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição ira retornar um JSON como este:

```json
[
  {
    "id": 1,
    "broker": null,
    "autonomous_agent": null,
    "trading_accounts": [],
    "name": "HSBC BANK BRASIL S.A. - BANCO MULTIPLO"
  },
  {
    "id": 2,
    "broker": null,
    "autonomous_agent": null,
    "trading_accounts": [],
    "name": "C.S.MENDES AGENTE AUTÔNOMO DE INVESTIMENTOS LTDA"
  },
  {
    "id": 3,
    "broker": null,
    "autonomous_agent": null,
    "trading_accounts": [],
    "name": "PREFEITURA DO MUNICÍPIO DE SÃO PAULO"
  }
]
```

Este recurso lista todas as instituições de um usuário autenticado.

### HTTP Request

`GET http://api.livecapital.com/users/{username}/institutions/custom`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
username | Nome de um usuário autenticado

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição do usuário
broker |
autonomous_agent |
trading_accounts |
name | Nome da instutuição do usuário

##POST /custom

```python
import urllib2

values = """
  {
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
    "uf": "SP",
    "ddd": "11"
  }
"""

headers = {
  'Content-Type': 'application/json'
}
request = urllib2.Request('http://api.livecapital.com/users/{username}/institutions/custom'.format(username), data=values, headers=headers)

response = urllib2.urlopen(request).read()

print response
```

> Essa requisição ira retornar um JSON como este:

```json
{
  "id": 1,
  "broker": null,
  "autonomous_agent": null,
  "trading_accounts": [],
  "name": "BANCO SANTANDER (BRASIL) S.A."
}
```

Este recurso cria uma instituição para um determinado usuário autenticado.

### HTTP Request

`POST http://api.livecapital.com/users/{username}/institutions/custom`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
username | Nome de um usuário autenticado

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição do usuário
broker |
autonomous_agent |
trading_accounts |
name | Nome da instutuição do usuário

##GET /custom/{id}

```python
from urllib2 import Request, urlopen

request = Request('http://api.livecapital.com/users/{}/institutions/custom/{}'.format(username, id))

response_body = urlopen(request).read()
print response_body
```

> Essa requisição ira retornar um JSON como este:

```json
{
  "id": 1,
  "broker": null,
  "autonomous_agent": null,
  "trading_accounts": [],
  "name": "BANCO SANTANDER (BRASIL) S.A."
}
```

Este recurso retorna uma determinada instituição de um usuário autenticado.
Será retornada a instituição com o id igual ao parâmetro passado na url.

### HTTP Request

`POST http://api.livecapital.com/users/{username}/institutions/custom/{id}`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
username | Nome de um usuário autenticado
id | Id de uma instituição de usuário

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição do usuário
broker |
autonomous_agent |
trading_accounts |
name | Nome da instutuição do usuário

##PUT /custom/{id}

```python
import urllib2

values = """
  {
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
    "uf": "SP",
    "ddd": "11"
  }
"""

opener = urllib2.build_opener(urllib2.HTTPHandler)
request = urllib2.Request('http://api.livecapital.com/institutions/custom/{id}', data=values)
request.add_header('Content-Type', 'application/json')
request.get_method = lambda: 'PUT'
response = opener.open(request)

print response.read()
```

> Essa requisição ira retornar um JSON como este:

```json
{
  "id": 1,
  "broker": null,
  "autonomous_agent": null,
  "trading_accounts": [],
  "name": "BANCO SANTANDER (BRASIL) S.A."
}
```

Este recurso altera/atualiza uma determinada instituição de um usuário autenticado.
Será alterada/atualizada a instituição com o id igual ao parâmetro passado na url.

### HTTP Request

`PUT http://api.livecapital.com/users/{username}/institutions/custom/{id}`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
username | Nome de um usuário autenticado
id | Id de uma instituição de usuário

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
id | Id da instituição do usuário
broker |
autonomous_agent |
trading_accounts |
name | Nome da instutuição do usuário

##DELETE /custom/{id}

```python
import urllib2

values = """
  {
    "id": 1,
    "broker": null,
    "autonomous_agent": null,
    "trading_accounts": [],
    "name": "BANCO SANTANDER (BRASIL) S.A."
  }
"""

opener = urllib2.build_opener(urllib2.HTTPHandler)
request = urllib2.Request('http://www.mocky.io/v2/5654ad7f0f00004c3160c1bc', data=values)
request.add_header('Content-Type', 'application/json')
request.get_method = lambda: 'DELETE'
response = opener.open(request)

print response.read()

```

Este recurso apaga uma determinada instituição de um usuário autenticado.
Será apagada a instituição com o id igual ao parâmetro passado na url.

### HTTP Request

`DELETE http://api.livecapital.com/users/{username}/institutions/custom/{id}`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
username | Nome de um usuário autenticado
id | Id de uma instituição de usuário
