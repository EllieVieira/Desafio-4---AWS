# Implementando Infraestrutura Automatizada com AWS CloudFormation

Este projeto faz parte do desafio **"Implementando Infraestrutura Automatizada com AWS CloudFormation"** da Digital Innovation One (DIO).  
O objetivo foi aplicar na prática os conceitos aprendidos sobre **Infraestrutura como Código (IaC)**, utilizando o **AWS CloudFormation** para automatizar a criação e o gerenciamento de recursos na nuvem.

---

## Objetivo do Desafio

Implementar uma infraestrutura automatizada com o **AWS CloudFormation**, documentando todo o processo, as etapas de criação e os aprendizados adquiridos durante o laboratório.

---

## Conceitos Principais

Durante a realização do desafio, revisei e coloquei em prática os seguintes conceitos:

- **Infraestrutura como Código (IaC):** permite automatizar e padronizar a criação de ambientes, reduzindo erros humanos e aumentando a eficiência.
- **AWS CloudFormation:** serviço da AWS que cria e gerencia recursos de forma automatizada através de templates em YAML ou JSON.
- **Stacks e Templates:**  
  - *Template:* arquivo que define todos os recursos a serem criados.  
  - *Stack:* conjunto de recursos implantados e gerenciados como uma única unidade.
- **Parâmetros, Recursos e Saídas:**  
  - *Parameters:* permitem personalizar as implantações.  
  - *Resources:* definem os serviços que serão criados.  
  - *Outputs:* mostram informações úteis ao final da criação da stack.
- **Diferença entre CloudFormation e Terraform:**  
  O CloudFormation é uma solução nativa da AWS, totalmente integrada aos seus serviços, enquanto o Terraform é multi-cloud e pode ser usado em diferentes provedores.

---

## Etapas Realizadas

### 1. Acesso ao AWS CloudFormation
Acessei o console da AWS e escolhi a opção de criar uma nova stack, podendo iniciar do zero ou fazer o upload de um template existente.

### 2. Criação do Template
Desenvolvi um template simples em formato **YAML**, responsável por criar um bucket S3 automaticamente.  
Segue o exemplo usado:

```yaml
AWSTemplateFormatVersion: '2010-09-09'
Description: Template simples para criação de um bucket S3

Resources:
  MeuBucketS3:
    Type: AWS::S3::Bucket
    Properties:
      BucketName: meu-bucket-cloudformation-exemplo
```

---

## Referências

- [Documentação Oficial do AWS CloudFormation](https://docs.aws.amazon.com/pt_br/AWSCloudFormation/latest/UserGuide/Welcome.html)   
- [Guia de Markdown no GitHub](https://guides.github.com/features/mastering-markdown/)

---

## Conclusão

A realização deste desafio consolidou o entendimento sobre Infraestrutura como Código (IaC) e mostrou a importância da automação no gerenciamento de ambientes em nuvem.  
O AWS CloudFormation se destacou como uma ferramenta poderosa e confiável para criar, manter e documentar ambientes de forma previsível e segura.
