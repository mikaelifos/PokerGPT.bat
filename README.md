# Aviso

Deixando claro: o texto abaixo partiu de um curso gratuito e ninguém tem autorização para redistribuí-lo. Se o assunto interessar, procure o curso aberto da trilha de Java com Spring Boot. Se a plataforma fechar o acesso ou passar a cobrar, não depende de mim — mas o material de lá é ótimo e quem assina um plano alcança bem mais.


# Geral

A aula usada como base foi a de gestão de dependências e build em Java com Maven.

Considerações gerais sobre extensões da ferramenta:

![general things about plugins in Maven](images/extensoes-em-geral.png)

As extensões mais usadas:

![most used plugins](images/extensoes-mais-usadas.png)

Como acionar uma extensão:

![how to use a plugin](images/como-usar-extensao.png)

Exemplo:

```
mvn dependency help
```

## Configuração de extensão

![plugin configuration](images/configuracao-de-extensao.png)

No começo a configuração é igual à de uma dependência:

- identificador do grupo;
- identificador do artefato;
- versão.

Depois vêm os ajustes específicos da extensão em uso, como o de publicação (veja a imagem).

## Exemplo de geração de documentação de código

Antes de tudo, acrescente a extensão de documentação ao arquivo de configuração do projeto.

![javadoc plugin install](images/instalando-extensao-doc.png)

Depois execute:

```
mvn javadoc:javadoc
```

Nesse ponto você já precisa ter os comentários de documentação nos lugares certos.

O resultado é gravado na pasta de artefatos gerados.

Exemplo do que é gerado:

![javadoc example](images/exemplo-de-documentacao.png)