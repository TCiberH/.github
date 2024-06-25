name: Relatório de Bug
description: Envie um relatório de bug.
title: "[Bug]: "
labels: ["bug", "triage"]
projects: ["octo-org/1", "octo-org/44"]
assignees:
  - octocat
body:
  - type: markdown
    attributes:
      value: |
        Obrigado por preencher este relatório de bug!
  - type: input
    id: contact
    attributes:
      label: Detalhes de Contato
      description: Como podemos entrar em contato com você se precisarmos de mais informações?
      placeholder: ex. email@example.com
      validations:
        required: false
  - type: textarea
    id: what-happened
    attributes:
      label: O que aconteceu?
      description: Também nos diga o que você esperava que acontecesse.
      placeholder: Conte-nos o que você viu!
      value: "Um bug aconteceu!"
      validations:
        required: true
  - type: dropdown
    id: version
    attributes:
      label: Versão
      description: Qual versão do nosso software você está usando?
      options:
        - 1.0.2 (Padrão)
        - 1.0.3 (Edge)
      default: 0
      validations:
        required: true
  - type: dropdown
    id: browsers
    attributes:
      label: Quais navegadores você está vendo o problema?
      multiple: true
      options:
        - Firefox
        - Chrome
        - Safari
        - Microsoft Edge
  - type: textarea
    id: logs
    attributes:
      label: Saída de log relevante
      description: Copie e cole qualquer saída de log relevante. Isso será formatado automaticamente como código.
      render: shell
  - type: checkboxes
    id: terms
    attributes:
      label: Código de Conduta
      description: Ao enviar este problema, você concorda em seguir nosso [Código de Conduta](https://bing.com/search?q=).
      options:
        - label: Concordo em seguir o Código de Conduta deste projeto
          required: true
