# Mega Man Robots API - Documentação

## Introdução
A **Mega Man Robots API** é um serviço backend desenvolvido em **.NET Core 3.1** que fornece dados formatados em JSON sobre os chefes da série **Mega Man**. A API foi desenvolvida com **Entity Framework Core** e outras tecnologias modernas do ecossistema .NET para garantir uma gestão eficiente dos dados e respostas otimizadas.

## Recursos
- **Fornece dados sobre robôs do universo Mega Man**.
- **Implementa padrão RESTful**, garantindo uma comunicação clara e eficiente.
- **Utiliza Entity Framework Core** para gerenciamento do banco de dados.
- **Aplicativo modular e escalável**, seguindo princípios de **injeção de dependência**.

## Endpoints da API
A API possui os seguintes endpoints disponíveis:

| Método | Endpoint             | Descrição                                      |
|---------|----------------------|------------------------------------------------|
| GET     | `/api/v1/robots`      | Retorna a lista de todos os robôs.           |
| GET     | `/api/v1/robots/{id}` | Retorna os detalhes de um robô específico.   |
| POST    | `/api/v1/robots`      | Cria um novo registro de robô.               |

## Tecnologias Utilizadas
A API foi desenvolvida utilizando:
- **Entity Framework Core**: ORM para manipulação de banco de dados.
- **RESTful API Design**: Padrão para comunicação entre sistemas.
- **Injeção de Dependência**: Garantindo desacoplamento e testabilidade.

## Dependências
A API depende dos seguintes pacotes NuGet:

| Pacote | Versão | Link |
|--------|--------|------|
| Microsoft.EntityFrameworkCore | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8) |
| Microsoft.EntityFrameworkCore.Design | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8) |
| Microsoft.EntityFrameworkCore.SqlServer | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8) |
| Newtonsoft.Json | 12.0.2 | [NuGet](https://www.nuget.org/packages/Newtonsoft.Json/12.0.2) |

## Estrutura do Projeto
O projeto está organizado da seguinte forma:

```
📂 src
├── 📂 Controllers      [Rotas para os endpoints]
├── 📂 Models           [Modelos de banco de dados]
├── 📂 Services         [Regras de negócio]
├── 📂 Middlewares      [Funções intermediárias no fluxo HTTP]
├── 📂 Database         [Estruturas relacionadas ao banco de dados]
│   ├── 📂 DTOs             [Modelos de entrada e saída (Data Transfer Objects)]
│   ├── 📂 EntityFramework  [Arquivos relacionados ao ORM Entity Framework]
│   │     ├── 📂 Context         [Configuração do contexto da entidade]
│   │     ├── 📂 Migrations      [Migrações para atualização do banco]
│   ├── 📂 Repositories     [Implementação do padrão Repository]
```

## Licença
Este software está licenciado sob os termos da **MIT License**.

Desenvolvido por **Felipe Aguiar** - [Github](https://github.com/felipeAguiarCode).

