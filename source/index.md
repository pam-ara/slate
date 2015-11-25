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
import urllib2

request = urllib2.Request('http://api.livecapital.com/clients/menu')
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de todas as instituições e suas contas.

### HTTP Request

`GET http://api.livecapital.com/clients/menu`

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |

##GET /accordions/{name}/{year}

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/clients/accordions/{}/{}'.format(name, year))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/accordions/{name}/{year}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/clients/accordions/{}/{}-{}'.format(name, year, month))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/accordions/{name}/{year}-{month}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/clients/operations/{}/{}'.format(name, year))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/operations/{name}/{year}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/clients/operations/{}/{}-{}'.format(name, year, month))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/operations/{name}/{year}-{month}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/clients/portfolios/{}/{}'.format(name, year))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/portfolios/{name}/{year}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/clients/portfolios/{}/{}-{}'.format(name, year, month))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/portfolios/{name}/{year}-{month}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/clients/returns/{}/{}'.format(name, year))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/returns/{name}/{year}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/clients/returns/{}/{}-{}'.format(name, year, month))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista

### HTTP Request

`GET http://api.livecapital.com/clients/returns/{name}/{year}-{month}`

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
[/institutions/official](#get-official) | GET | Lista todas as instituinções oficiais
[/institutions/official/{id}](#get-official-id) | GET | Retorna uma instituição oficial específica
[/institutions/custom](#get-custom) | GET | Lista todas as instituições de um usuário autenticado
[/institutions/custom](#post-custom) | POST | Cria uma instituição para um usuário
[/institutions/custom/{id}](#get-custom-id) | GET | Retorna uma determinada instituição de um usuário
[/institutions/custom/{id}](#put-custom-id) | PUT | Atualiza/Altera dados de uma instituição
[/institutions/custom/{id}](#delete-custom-id) | DELETE | Apaga uma instituição


##GET /official

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/institutions/official')
response = urllib2.urlopen(request).read()

print response
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
  "uf": "SP",
  "ddd": "11"
}
```

Esse recurso retorna uma instituição específica.

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
category | Tipo de instituição. Existem apenas as categorias "BROKER" e "AUTONOMOUS_AGENT".
person_type | Tipo de pessoa
identifier | Número identificador
social_denomination | Denominação social
commercial_denomination | Denominação comercial

##GET /custom

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/users/{}/institutions/custom'.format(username))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

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
request = urllib2.Request('http://api.livecapital.com/users/{}/institutions/custom'.format(username), data=values, headers=headers)

response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/users/{}/institutions/custom/{}'.format(username, id))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

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
request = urllib2.Request('http://api.livecapital.com/institutions/custom/{}'.format(id), data=values)
request.add_header('Content-Type', 'application/json')
request.get_method = lambda: 'PUT'
response = opener.open(request)

print response.read()
```

> Essa requisição irá retornar um JSON como este:

```json
{
  "id": 1,
  "broker": null,
  "autonomous_agent": null,
  "trading_accounts": [],
  "name": "BANCO SANTANDER (BRASIL) S.A."
}
```

Este recurso altera uma determinada instituição de um usuário autenticado.

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
request = urllib2.Request('http://api.livecapital.com/users/{}instittutions/custom/{}'.format(username, id), data=values)
request.add_header('Content-Type', 'application/json')
request.get_method = lambda: 'DELETE'
response = opener.open(request)

print response.read()

```

Este recurso apaga uma determinada instituição de um usuário autenticado.

### HTTP Request

`DELETE http://api.livecapital.com/users/{username}/institutions/custom/{id}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/darf/{}-{}/reports'.format(year, month))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso exibe um relatório filtrado por mês e ano.

### HTTP Request

`GET http://api.livecapital.com/darf/{year}-{month}/reports`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/darf/{}-{}/print'.format(year, month))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso exibe uma DARF filtrada por mês e ano.

### HTTP Request

`GET http://api.livecapital.com/darf/{year}-{month}/print`

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

Esses são todos os recursos de Bovespa disponíveis.

Recurso | Método | Descrição
------- | ------ | ---------
[/bovespa/trading-account](#get-trading-account) | GET | Lista todas as contas de um usuário autenticado
[/bovespa/trading-account](#post-trading-account) | POST | Cria uma conta de Bovesta para um usuário autenticado
[/bovespa/trading-account/{id}](#get-trading-account-id) | GET | Exibe os dados de uma conta
[/bovespa/assets](#get-assets) | GET | Retorna uma lista de ativos
[/bovespa/brokerage-notes](#post-brokerage-notes) | POST | Cria uma nota de corretagem
[/bovespa/brokerage-notes/{id}](#get-brokerage-notes-id) | GET | Exibe dados da nota de corretagem
[/bovespa/brokerage-notes/{id}](#put-brokerage-notes-id) | PUT | Altera dados da nota de corretagem
[/bovespa/brokerage-notes/{id}](#delete-brokerage-notes-id) | DELETE | Apaga uma nota de corretagem
[/bovespa/positions/{date}/terms](#get-positions-date-terms) | GET | Retorna a posição da conta na data informada apenas por termos
[/bovespa/positions/{date}/non-terms](#get-positions-date-non-terms) | GET | Retorna a posição da conta na data informada sem termos
[/bovespa/events/{trading-account}/{date}](#get-trading-account-date) | GET | Lista todos os eventos de uma conta filtrados por data
[/bovespa/{event_type}/{id}](#get-event-type-id) | GET | Exibe dados de um evento
[/bovespa/{event_type}/{id}](#put-event-type-id) | PUT | Altera dados de um evento
[/bovespa/{event_type}/{id}](#delete-event-type-id) | DELETE | Apaga um evento

##GET /trading-account

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/bovespa/trading-account')
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso lista todas as contas de um usuário autenticado.

### HTTP Request

`GET http://api.livecapital.com/bovespa/trading-account`

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |

##POST /trading-account

```python
import urllib2

values = """
  {
  }
"""

headers = {
  'Content-Type': 'application/json'
}
request = urllib2.Request('http://api.livecapital.com/bovespa/trading-account', data=values, headers=headers)

response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso cria uma conta Bovespa para um usuário autenticado.

### HTTP Request

`POST http://api.livecapital.com/bovespa/trading-account`

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |

##GET /trading-account/{id}

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/bovespa/trading-account/{}'.format(id))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna dados de uma conta bovespa.

### HTTP Request

`GET http://api.livecapital.com/bovespa/trading-account/{id}`

### Parâmetros de URL

Parâmetro | Descrição
--------- | ---------
id | Id de uma conta

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |

##GET /assets

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/assets')
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de ativos.

### HTTP Request

`GET http://api.livecapital.com/bovespa/assets`

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |

##POST /brokerage-notes

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/bovespa/brokerage-notes')
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso cria uma nota de corretagem.

### HTTP Request

`POST http://api.livecapital.com/bovespa/brokerage-notes`

### Parâmetros de resposta

Parâmetro | Descrição
--------- | ---------
 |
 |
 |

##GET /brokerage-notes/{id}

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/bovespa/brokerage-notes/{}'.format(id))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna os dados de uma nota de corretagem.

### HTTP Request

`GET http://api.livecapital.com/bovespa/brokerage-notes/{id}`

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

##PUT /brokerage-notes/{id}

```python
import urllib2

values = """
  {
  }
"""

opener = urllib2.build_opener(urllib2.HTTPHandler)
request = urllib2.Request('http://api.livecapital.com/bovespa/brokerage-notes/{}'.format(id), data=values)
request.add_header('Content-Type', 'application/json')
request.get_method = lambda: 'PUT'
response = opener.open(request)

print response.read()
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso altera dados de uma nota de corretagem.

### HTTP Request

`PUT http://api.livecapital.com/bovespa/brokerage-notes/{id}`

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

##DELETE /brokerage-notes/{id}

```python
import urllib2

opener = urllib2.build_opener(urllib2.HTTPHandler)
request = urllib2.Request('http://api.livecapital.com/bovespa/brokerege-notes/{}'.format(id))
request.add_header('Content-Type', 'application/json')
request.get_method = lambda: 'DELETE'
response = opener.open(request)

print response.read()

```

Esse recurso apaga uma nota de corretagem.

### HTTP Request

`DELETE http://api.livecapital.com/bovespa/brokerage-notes/{id}`

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

##GET /positions/{date}/terms

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/bovespa/positions/{}/terms'.format(date))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna a posição da conta na data informada exibindo apenas os termos.

### HTTP Request

`GET http://api.livecapital.com/bovespa/positions/{date}/terms`

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

##GET /positions/{date}/non-terms

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/bovespa/positions/{}/non-terms'.format(date))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna a posição da conta na data informada, mas não exibe os termos.

### HTTP Request

`GET http://api.livecapital.com/bovespa/positions/{date}/non-terms`

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

##GET /events/{trading-account}/{date}

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/bovespa/events/{}/{}'.format(trading-account, date))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso lista todos os eventos de uma conta filtrando por data.

### HTTP Request

`GET http://api.livecapital.com/bovespa/events/{trading-account}/{date}`

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

##GET /{event_type}/{id}

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/bovespa/{}/{}'.format(event-type, id))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna dados de um evento.

### HTTP Request

`GET http://api.livecapital.com/bovespa/{event-type}/{id}`

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

##PUT /{event_type}/{id}

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/bovespa/{}/{}'.format(event-type, id))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso altera dados de um evento.

### HTTP Request

`PUT http://api.livecapital.com/bovespa/{event-type}/{id}`

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

##DELETE /{event_type}/{id}

```python
import urllib2

request = urllib2.Request('http://api.livecapital.com/bovespa/{}/{}'.format(event_type, id))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso apaga um evento.

### HTTP Request

`GET http://api.livecapital.com/bovespa/{event-type}/{id}`

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

#Widgets

##Recursos

Esses são todos os recursos de widgets disponíveis.

Recurso | Método | Descrição
------- | ------ | ---------
[/widgets/{name}/{market}/{year}](#get-name-market-year) | GET | Retorna uma lista de widgets filtrados por um ano
[/widgets/{name}/{market}/{year}-{month}](#get-name-market-year-month) | GET | Retorna uma lista de widgets filtrados por um mês e ano
[/widgets/{name}/{market}/{year}-{month}-{day}](#get-name-market-year-month-day) | GET | Retorna uma lista de widgets filtrados por uma data
[/widgets/portfolios/{year}](#get-portfolios-name-market-year47) | GET | Retorna uma lista de widgets portfolios filtrados por ano
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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/{}/{}/{}'.format(name, market, year))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets de determinado nome filtrados por um ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/{name}/{market}/{year}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/{}/{}/{}-{}'.format(name, market, year, month))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets de determinado nome filtrados por mês e ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/{name}/{market}/{year}-{month}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/{}/{}/{}-{}-{}'.format(name, market, year, month, day))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets de determinado nome filtrados por uma data.

### HTTP Request

`GET http://api.livecapital.com/widgets/{name}/{market}/{year}-{month}-{day}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/portfolios/{}'.format(year))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets portfolio filtrados por um ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/portfolios/{year}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/portfolios/{}-{}'.format(year, month))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets portfolio filtrados por um mês e ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/portfolios/{year}-{month}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/portfolios/{}-{}-{}'.format(year, month, day))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets portfolio filtrados por uma data.

### HTTP Request

`GET http://api.livecapital.com/widgets/portfolios/{year}-{month}-{day}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/capital-gain/{}'.format(year))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets capital-gain filtrados por um ano.

### HTTP Request

`GET http://api.livecapital.com/wigets/capital-gain/{year}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/capital-gain/{}-{}'.format(year, month))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets capital-gain filtrados por um mês e ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/capital-gain/{year}-{month}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/capital-gain/{}-{}-{}'.format(year, month, day))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets capital-gain filtrados por uma data.

### HTTP Request

`GET http://api.livecapital.com/widgets/capital-gain/{year}-{month}-{day}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/taxes/{}'.format(year))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets taxes filtrados por um ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/taxes/{year}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/taxes/{}-{}'.format(year, month))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets taxes filtrados por um mês e ano.

### HTTP Request

`GET http://api.livecapital.com/widgets/taxes/{year}-{month}`

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
import urllib2

request = urllib2.Request('http://api.livecapital.com/widgets/taxes/{}-{}-{}'.format(year, month, day))
response = urllib2.urlopen(request).read()

print response
```

> Essa requisição irá retornar um JSON como este:

```json
```

Esse recurso retorna uma lista de widgets taxes filtrados por uma data.

### HTTP Request

`GET http://api.livecapital.com/widgets/taxes/{year}-{month}-{day}`

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
