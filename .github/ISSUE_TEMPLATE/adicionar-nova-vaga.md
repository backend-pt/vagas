name: Adicionar nova vaga
description: Não esqueça de seguir todas as instruções do template antes de abrir a vaga.
title: '[Cidade] Título da Vaga @ Nome da Empresa'
body:
  - type: markdown
    attributes:
      value: |
        ## :warning: Observações

        - Só publique vagas para back-end
        - Não faça destinção de gênero no título da vaga
        - Use: "Pessoa desenvolvedora" ou "Backend Developer" ao invés de "Desenvolvedor Back-End" \o/

        ---

  - type: textarea
    validations:
      required: true
    attributes:
      label: Nossa empresa
      placeholder: 'Exemplo: Aqui na Corporação ACME somos líderes em...'

  - type: textarea
    validations:
      required: true
    attributes:
      label: Descrição da vaga
      placeholder: 'Exemplo: Projeto bazinga em NestJS, etc.'

  - type: textarea
    validations:
      required: true
    attributes:
      label: Local
      placeholder: 'Exemplo: Remoto ou Escritório, São Paulo - Vila Olímpia'

  - type: textarea
    validations:
      required: true
    attributes:
      label: Requisitos
      value: |
        #### Obrigatórios:
        - 2 anos de experiência com NestJS
        - 2 anos de experiência com mongodb

        ### Desejáveis:
        - conhecimentos em Docker
        - conhecimentos em AWS

        ### Diferenciais:
        - projetos open source

  - type: textarea
    validations:
      required: true
    attributes:
      label: Benefícios
      value: |
        - Plano de saúde
        - Seguro de vida
        - VR de R$ X/dia
        - Auxílio creche
        - ...

        #### Diferenciais
        - 2 horas de almoço
        - monte a sua máquina como desejar
        - frigobar sempre cheio :P
        - sala de jogos
        - ...

  - type: input
    validations:
      required: true
    attributes:
      label: Contratação
      placeholder: PJ a combinar

  - type: input
    validations:
      required: true
    attributes:
      label: Como se candidatar
      placeholder: |
        Por favor envie um email para email@email.com.br com seu CV anexado - enviar no assunto: Vaga NestJS

  - type: input
    validations:
      required: false
    attributes:
      label: Tempo médio de feedbacks
      placeholder: |
        Costumamos enviar feedbacks em até XX dias após cada processo.

  - type: markdown
    attributes:
      value: |
        ## Labels

  - type: input
    validations:
      required: false
    attributes:
      label: Keywords
      placeholder: nestjs mysql

  - type: checkboxes
    attributes:
      label: Alocação
      options:
        - label: Alocado
          required: false
        - label: Remoto
          required: false
        - label: Presencial
          required: false
        - label: Híbrido
          required: false

  - type: checkboxes
    attributes:
      label: Regime
      options:
        - label: CLT
          required: false
        - label: Estágio
          required: false
        - label: Freela
          required: false
        - label: PJ
          required: false
        - label: Cooperado
          required: false

  - type: checkboxes
    attributes:
      label: Nível
      options:
        - label: Júnior
          required: false
        - label: Pleno
          required: false
        - label: Sênior
          required: false
        - label: Especialista
          required: false
          
  - type: checkboxes
    attributes:
      label: Período
      options:
        - label: Full time
          required: false
        - label: Part Time
          required: false
        - label: Projeto
          required: false
          
  - type: dropdown
    attributes:
      label: Remuneração
      options:
        - R$ 1k - R$ 5k
        - R$ 5k - R$ 10k
        - R$ 10k - R$ 15k
        - R$ 15k - R$ 20k
        - R$ 20k+
    validations:
      required: false
