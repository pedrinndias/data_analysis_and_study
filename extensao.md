# Modelo de Dados da Farmácia

Este é o Diagrama de Entidade-Relacionamento para o sistema da farmácia.

```mermaid
erDiagram
    %% Entidades Principais
    Farmacia {
        string CNPJ PK "Chave Primária"
        string Nome
        string Endereco
    }

    Cliente {
        string CPF PK "Chave Primária"
        string Nome
        date Data_Nascimento
        int Idade "Derivado"
        string Telefones "Multivalorado"
        string Endereco "Composto"
    }

    Nota_Fiscal {
        int Numero_NF PK "Chave Primária"
        date Data_Emissao
        float Valor_Total
    }

    %% Entidade Associativa para N:M
    Item_Nota {
        int Quantidade_Comprada
    }

    %% Entidades com Herança (Generalização/Especialização)
    Funcionario {
        int Matricula PK "Chave Primária"
        string Nome
        string Cargo
        float Salario
    }

    Farmaceutico {
        string Num_Conselho_Profissional
    }

    Atendente {
        float Percentual_Comissao
    }

    Gerente {
        float Volume_Vendas
    }

    Produto {
        int Codigo PK "Chave Primária"
        string Descricao
        float Preco_Unitario
        int Qtde_em_Estoque
    }

    Remedio {
        date Data_Validade
        bool Obrigat_Receita
    }


    %% Relacionamentos
    Farmacia ||--|{ Funcionario : "possui"
    Farmacia ||--|{ Nota_Fiscal : "emite"
    Cliente ||--|{ Nota_Fiscal : "realiza_compra"

    %% Relacionamento N:M via Entidade Associativa
    Nota_Fiscal ||--|{ Item_Nota : "contém"
    Produto ||--|{ Item_Nota : "é_item_de"

    %% Relacionamentos de Herança (ISA)
    %% Funcionário -> Total e Disjunta
    Funcionario ||--|> Farmaceutico
    Funcionario ||--|> Atendente
    Funcionario ||--|> Gerente

    %% Produto -> Parcial
    Produto ||--|> Remedio
