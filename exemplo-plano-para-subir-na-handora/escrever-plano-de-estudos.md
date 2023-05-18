# Escrevendo plano de estudos

## Formato do json para um novo plano

Este repositório tem vários exemplos de json, pois são os jsons que foram usados para cadastrar os planos que estão atualmente na plataforma.

A handora tem um endpoint para cadastrar um json que representa um plano de estudos. O json tem a seguinte estrutura:

```json
{
  "titulo": "Meu plano de estudos",
  "motivacao": "Esse plano é importante pelo seguinte...",
  "objetivo": "os objetivos do plano\n\nmais um objetivo aqui com quebra de linha\n\n**da pra usar markdown também**",
  "palavrasChave": [
    "application",
    "palavra 1",
    "palavra 2",
    "palavra n",
  ],
  "temas": [
    {
      "titulo": "tema 1",
      "referencias": [
        {
          "titulo": "Referencia do tema 1",
          "url": "https://referencia.com"
        }
      ],
      "habilidades": [
        "Ser capaz de virar o novo primeiro volante do Vasco",
        "Aprender mais sobre assunto xpto"
      ],
      "formasVerificacaoConhecimento": [
        {
          "titulo": "Faça um resumo",
          "url": "https://typeform.com/resumo"
        }
      ]
    }
  ],
  "formasValidacaoConhecimento": [
    {
      "titulo": "Será que agora você consegue construir uma stack completa para compartilhar seu conhecimento via Stackspot?",
      "url": "https://zup1.typeform.com/to/q8lD8vcv"
    }
  ]
}
```

### Valores obrigatórios

O que é opcional aí:

- `formasValidacaoConhecimento`
- `formasVerificacaoConhecimento`

Todas as outras chaves do json são obrigatórias, seja no plano de estudos como um todo, seja em cada tema.

### Titúlos repetidos

Não pode haver repetição de valores, por exemplo títulos de referências repetidos no mesmo tema etc.
