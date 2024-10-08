
# My Building Block (Schema)

`avillar.sandbox.my-building-block` *v0.1*

This Building Block serves as a template to create new ones

[*Status*](http://www.opengis.net/def/status): Under development

## Description

## Qui hastarum tectus Cithaeron iuvabat

Lorem markdownum vestigia sanguine rursus undis, suspenderat meo mox conlegerat
temperat sucos. Est graves dant sentire sanguinis flores respondent testari.

** This is a relative URL: [example.png](assets/example.png) **.

![Image](assets/example.png)

> Videri vias quid Ausoniae sua flores ante, reminiscitur fuit est. Semel
> [hectora](http://silvaque.org/) peregrinaeque rudem exercent in, Troiana si
> Asida instabilesque somno sed.

## Iam vota cui dilataque peterem

Tinxit lumina lacer liquidarum Aiax si mergitur sed fueris capitisque **et
cadit** contigerant rectum [ferar](http://prosternit.com/quoque.html) temperat.
Monet caput adsensere Ityn furentibus gelidos.
## Examples

### This is an example with just a description and no code snippets.
This is the content of the example.

In **Markdown** format.

** This is a relative URL: [example.png](assets/example.png) **.

![Image](assets/example.png)

### Examples can have content and/or code snippets.
The content of this example. 

** This is a relative URL: [example.png](assets/example.png) **.

![Image](assets/example.png)
#### shell
```shell
echo 'Hello, world!'
```

#### python
```python
print('Hello, world!')
```

#### javascript
```javascript
console.log('Hello, world!')
```


### JSON Example
#### json
```json
{
  "a": "http://www.google.es",
  "b": 33,
  "d": "agreed"
}
```

#### jsonld
```jsonld
{
  "a": "http://www.google.es",
  "b": 198,
  "d": "agreed",
  "@context": "https://avillar.github.io/bblocks-sandbox/build/annotated/sandbox/my-building-block/context.jsonld"
}
```

#### ttl
```ttl
@prefix ns1: <https://example.org/my-bb-model/> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

[] ns1:a <http://www.google.es> ;
    ns1:aalias <http://www.google.es> ;
    ns1:b 198 ;
    ns1:bnew 396.0 .


```


### RDF Example with prefixes
#### ttl
```ttl
ex:a dct:title ex:b .
```


### JSON Example with prefixes
#### json
```json
{
  "dct:title": "Juan"
}
```


### JSON-LD Example with prefixes
#### jsonld
```jsonld
{
  "@context": {
    "q": "http://q.net/"
  },
  "q:a": "bcd",
  "dct:title": "Juan"
}
```

#### ttl
```ttl


```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: Schema for my building block
type: object
$defs:
  test:
    type: string
properties:
  a:
    type: string
    format: uri
    x-jsonld-id: https://example.org/my-bb-model/a
    x-jsonld-type: '@id'
  b:
    type: number
    x-jsonld-id: https://example.org/my-bb-model/b
  c:
    $ref: https://avillar.github.io/bblocks-sandbox/build/annotated/sandbox/my-building-block/schema.yaml#/$defs/test
  d:
    $ref: https://avillar.github.io/bblocks-sandbox/build/annotated/sandbox/enumerations/legalStatus/schema.yaml
required:
- a
- b

```

Links to the schema:

* YAML version: [schema.yaml](https://avillar.github.io/bblocks-sandbox/build/annotated/sandbox/my-building-block/schema.json)
* JSON version: [schema.json](https://avillar.github.io/bblocks-sandbox/build/annotated/sandbox/my-building-block/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "a": {
      "@id": "https://example.org/my-bb-model/a",
      "@type": "@id"
    },
    "b": "https://example.org/my-bb-model/b",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://avillar.github.io/bblocks-sandbox/build/annotated/sandbox/my-building-block/context.jsonld)

## Sources

* [Sample source document](https://example.com/sources/1)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/avillar/bblocks-sandbox](https://github.com/avillar/bblocks-sandbox)
* Path: `_sources/my-building-block`

