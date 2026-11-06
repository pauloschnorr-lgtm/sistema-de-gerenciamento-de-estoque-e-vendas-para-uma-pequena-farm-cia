# sistema-de-gerenciamento-de-estoque-e-vendas-para-uma-pequena-farmacia
Sistema de Estoque e Vendas para Farmácia (C++)

Programa de terminal em C++ para gerenciar o estoque e as vendas de uma pequena farmácia. Trabalho da disciplina de Algoritmos e Programação 1 do curso de Ciência da Computação da Univali.

Por exigência do trabalho, o programa usa apenas decisões, laços de repetição e vetores, sem funções, structs ou classes. Os dados de cada medicamento ficam em três vetores paralelos (nome, quantidade e preço), ligados pelo mesmo índice.

Funcionalidades

O sistema tem um menu com 6 opções:

Opção	O que faz
1 - Cadastrar medicamento	Cadastra nome, quantidade em estoque e preço unitário
2 - Atualizar estoque	Soma uma quantidade ao estoque de um medicamento já cadastrado
3 - Buscar medicamento	Procura pelo nome e mostra nome, quantidade e preço
4 - Vender medicamentos	Registra uma venda com vários medicamentos e mostra o total
5 - Listar medicamentos	Lista todos os medicamentos e o valor total do estoque
6 - Sair	Encerra o programa
Regras e validações
Limite de 50 medicamentos cadastrados
Nome único: não permite cadastrar dois medicamentos com o mesmo nome
Quantidade e preço devem ser maiores que zero, e o programa pede o valor de novo até ser válido
Na venda, se a quantidade pedida for maior que o estoque, o programa avisa e pede outra quantidade, então o estoque nunca fica negativo
A venda continua enquanto o usuário responder S à pergunta "Outro medicamento? S/N"
Valores em reais são exibidos com 2 casas decimais
Como compilar e executar

Requer um compilador C++ (por exemplo, o g++).

bash
g++ PauloRafaelM3.cpp -o farmacia
./farmacia

No Windows, execute farmacia.exe.

Exemplo de uso
*GERENCIAMENTO DE ESTOQUE*
Escolha uma opção:
 1 - Cadastrar medicamento
 2 - Atualizar estoque
 3 - Buscar medicamento
 4 - Vender medicamentos
 5 - Listar medicamentos cadastrados
 6 - Sair
Conceitos aplicados
Vetores paralelos para armazenar os dados
Busca sequencial em vetor
Estruturas de decisão e laços (do-while, for, while)
Validação de entrada de dados
Formatação de saída com iomanip (fixed e setprecision)
Melhorias planejadas
Aceitar nomes com mais de uma palavra (hoje a leitura usa cin >>, que para no primeiro espaço)
Tratar entradas que não sejam números, para o programa não travar
Validar a resposta S/N na venda
Separar o código em funções e usar struct para agrupar os dados do medicamento
Salvar os dados em arquivo para não perder o estoque ao fechar o programa
Autores
Paulo Conceição
