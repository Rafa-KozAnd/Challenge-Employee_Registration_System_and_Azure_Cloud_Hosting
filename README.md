<p align="center">
  <img src="http://img.shields.io/static/v1?label=STATUS&message=Concluded&color=blue&style=flat"/>
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/Rafa-KozAnd/Challenge-Employee_Registration_System_and_Azure_Cloud_Hosting">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/top/Rafa-KozAnd/Challenge-Employee_Registration_System_and_Azure_Cloud_Hosting">
  <img alt="GitHub repo file count" src="https://img.shields.io/github/directory-file-count/Rafa-KozAnd/Challenge-Employee_Registration_System_and_Azure_Cloud_Hosting">
  <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Rafa-KozAnd/Challenge-Employee_Registration_System_and_Azure_Cloud_Hosting">
  <img alt="GitHub language count" src="https://img.shields.io/github/license/Rafa-KozAnd/Challenge-Employee_Registration_System_and_Azure_Cloud_Hosting">
</p>

# Challenge-Employee_Registration_System_and_Azure_Cloud_Hosting

- Project Name: 'Challenge-Employee_Registration_System_and_Azure_Cloud_Hosting';
- Languages: 'C#';
- Softwares/Work Tools: 'V.S. Code';
- Resume: ;
- Obs: Example;
- Version: v.1.0.0

- Last Update Date: 17/09/2024.

##


# DIO - Trilha .NET - Nuvem com Microsoft Azure
www.dio.me

## Desafio de projeto
Para este desafio, você precisará usar seus conhecimentos adquiridos no módulo de Nuvem com Microsoft Azure, da trilha .NET da DIO.

## Contexto
Você precisa construir um sistema de RH, onde para essa versão inicial do sistema o usuário poderá cadastrar os funcionários de uma empresa. 

Essa cadastro precisa precisa ter um CRUD, ou seja, deverá permitir obter os registros, criar, salvar e deletar esses registros. A sua aplicação também precisa armazenar logs de toda e qualquer alteração que venha a ocorrer com um funcionário.

## Premissas
A sua aplicação deverá ser do tipo Web API, Azure Functions ou MVC, fique a vontade para implementar a solução que achar mais adequado.

A sua aplicação deverá ser implantada no Microsoft Azure, utilizando o App Service para a API, SQL Database para o banco relacional e Azure Table para armazenar os logs.

A sua aplicação deverá armazenar os logs de todas as alterações que venha a acontecer com o funcionário. Os logs deverão serem armazenados em uma Azure Table.

A sua classe principal, a classe Funcionario e a FuncionarioLog, deve ser a seguinte:

![Diagrama da classe Funcionario](Imagens/diagrama_classe.png)

A classe FuncionarioLog é filha da classe Funcionario, pois o log terá as mesmas informações da Funcionario.

Não se esqueça de gerar a sua migration para atualização no banco de dados.

## Métodos esperados
É esperado que você crie o seus métodos conforme a seguir:


**Swagger**


![Métodos Swagger](Imagens/swagger.png)


**Endpoints**


| Verbo  | Endpoint                | Parâmetro | Body               |
|--------|-------------------------|-----------|--------------------|
| GET    | /Funcionario/{id}       | id        | N/A                |
| PUT    | /Funcionario/{id}       | id        | Schema Funcionario |
| DELETE | /Funcionario/{id}       | id        | N/A                |
| POST   | /Funcionario            | N/A       | Schema Funcionario |

Esse é o schema (model) de Funcionario, utilizado para passar para os métodos que exigirem:

```json
{
  "nome": "Nome funcionario",
  "endereco": "Rua 1234",
  "ramal": "1234",
  "emailProfissional": "email@email.com",
  "departamento": "TI",
  "salario": 1000,
  "dataAdmissao": "2022-06-23T02:58:36.345Z"
}
```

## Ambiente
Este é um diagrama do ambiente que deverá ser montado no Microsoft Azure, utilizando o App Service para a API, SQL Database para o banco relacional e Azure Table para armazenar os logs.

![Diagrama da classe Funcionario](Imagens/diagrama_api.png)


## Solução
O código está pela metade, e você deverá dar continuidade obedecendo as regras descritas acima, para que no final, tenhamos um programa funcional. Procure pela palavra comentada "TODO" no código, em seguida, implemente conforme as regras acima, incluindo a sua publicação na nuvem.