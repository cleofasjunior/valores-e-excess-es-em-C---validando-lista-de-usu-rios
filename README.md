📝 Manipulação e Validação de Nomes em C#
Tratando Entradas e Erros em Listas de Strings

📌 Descrição

Este projeto implementa um programa em C# para processar uma lista de nomes inseridos pelo usuário. O sistema realiza:

A leitura e separação de nomes digitados pelo usuário, considerando vírgulas como delimitadores.

A remoção de espaços extras e aspas desnecessárias.

A validação de entradas para detectar nomes inválidos, como:

"null" explícito;

strings nulas, vazias ou contendo apenas espaços.

Ao final, o programa exibe uma saída formatada contendo:

A lista de nomes válidos;

As mensagens de erros encontrados (se houver).

📝 Entrada

O programa recebe uma única linha contendo nomes separados por vírgula.

Exemplo de entrada válida:

"Ana, Pedro, null, , João"

📤 Saída

O programa retorna uma string contendo:

Apenas nomes válidos, se não houver erros.

Nomes válidos acompanhados das mensagens de erro, se houver inconsistências.

Formato esperado:

[nomes válidos] / [mensagens de erro]

📊 Exemplos de execução
Entrada	Saída
Ana, Pedro, João	Ana, Pedro, João
Maria, null, José	Maria, José / Erro: nome nulo
"", Joana, , Carlos	Joana, Carlos / Erro: nome invalido
null, ,	Erro: nome nulo / Erro: nome invalido
⚙️ Estrutura do Projeto

O código foi desenvolvido em C#, utilizando conceitos como:

Listas genéricas (List<T>) para armazenar nomes válidos e erros.

LINQ para facilitar o processamento inicial das entradas.

Validações condicionais (if/else) para detectar inconsistências.

Manipulação de strings para remoção de espaços e aspas.

🖼️ Diagrama do Projeto

▶️ Como Executar

Clone o repositório:

git clone https://github.com/seu-usuario/validacao-nomes.git


Acesse a pasta do projeto:

cd validacao-nomes


Compile e execute o programa em C#:

dotnet run

🚀 Tecnologias Utilizadas

Linguagem: C#

Paradigma: Programação Orientada a Objetos (POO) + LINQ

Framework: .NET

📚 Habilidades e Aprendizados Desenvolvidos

Durante o desenvolvimento deste projeto, foram explorados e praticados os seguintes aspectos:

Uso de listas genéricas (List<T>) para manipular coleções.

Aplicação de LINQ para transformar entradas em dados processáveis.

Implementação de validações condicionais robustas.

Tratamento de entradas inválidas e erros de lógica.

Consolidação de boas práticas no processamento de strings.

📌 Principais Competências

✔️ Manipulação e validação de listas de strings
✔️ Uso prático de LINQ em C#
✔️ Separação entre entrada, processamento e saída
✔️ Exibição de resultados padronizados e claros
✔️ Tratamento de casos especiais e valores inválidos


🔧 Pontos de Melhoria

Embora funcional, o projeto pode ser estendido com as seguintes melhorias:

Adicionar tratamento de exceções para entradas nulas.

Permitir leitura de nomes a partir de arquivos externos.

Criar uma versão que suporte interface gráfica para melhor usabilidade.

Implementar testes automatizados para validar os cenários possíveis.

Expandir o sistema para categorizar nomes válidos e inválidos em relatórios.
