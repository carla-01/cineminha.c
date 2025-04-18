# CINEMINHA
## Descrição Técnica
Este módulo é responsável pelo gerenciamento de memória em um sistema de reservas de cinema, com foco na liberação segura de estruturas alocadas dinamicamente.

### Funcionalidades Principais

#### Gerenciamento de Memória

    Liberação de strings de poltronas reservadas

    Desalocação do array de poltronas

    Liberação da estrutura principal de pedidos

    Tratamento de casos onde o pedido não é encontrado

#### Interface do Usuário
    Mensagens de feedback coloridas (ANSI)

    Validação de entrada do usuário

    Mensagem de saída do sistema
    
    Estrutura do Código

         c// Exemplo da lógica de liberação

         for(int i = 0; i < p->numPoltronas; i++) {

         printf("Poltrona: %s\n", p->poltronas[i]);

         free(p->poltronas[i]);  // Libera cada string de poltrona
         }
         free(p->poltronas);  // Libera o array de ponteiros

         free(p);  // Libera a estrutura principal

    Compilação e Uso

#### Requisitos do Sistema
    Compilador C (GCC recomendado)

    Suporte a alocação dinâmica

    Terminal com suporte a cores ANSI

#### Dependências
    Definição da estrutura pedido

    Funções auxiliares para manipulação de CSV


#### Interface:

    Cores ANSI para melhor experiência do usuário

    Mensagens claras de erro/sucesso

#### Integração:

    Parte de um sistema maior de reservas

    Projetado para trabalhar com arquivos CSV

