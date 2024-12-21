# 2024.2 Avaliação do 1o período de Sistemas Operacionais

## Informações gerais
- **Objetivo do repositório**: Avaliação do 1o bimestre da Disciplina de sistemas operacionais do curso de TADS do IFRN-CNAT
- **Público alvo**: alunos da disciplina de SO (Sistemas Operacionais) do curso de TADS (Superior em Tecnologia em Análise e Desenvolvimento de Sistemas) no CNAT-IFRN (Instituto Federal de Educação, Ciência e Tecnologia do Rio Grande do Norte - Campus Natal-Central).
- disciplina: **SO** Sistemas Operacionais
- professor: [Leonardo A. Minora](https://github.com/leonardo-minora)

## Avaliação
- **Lembre de fazer o fork deste repositório**
- As questões foram construídas com o auxílio do [copilot](https://copilot.microsoft.com/)

# Questão 1. Introdução a sistemas operacionais

Considere as funções e objetivos principais de um sistema operacional conforme discutido no texto. Explique como um sistema operacional gerencia os recursos de hardware e software de um computador para garantir eficiência e segurança. Em sua resposta, aborde os seguintes pontos:

- Gerenciamento de processos
- Gerenciamento de memória
- Gerenciamento de dispositivos de entrada e saída
- Gerenciamento de arquivos

**Dica**: Pense em exemplos práticos de como o sistema operacional realiza essas tarefas no dia a dia de um usuário.

**Copilot informa**: Essa questão incentiva os alunos a explorarem os conceitos fundamentais e a aplicarem o conhecimento teórico em situações práticas. Se precisar de mais alguma coisa, estou aqui para ajudar!

# Questão 1 - Resposta
O sistema operacional é como o "chefe" do computador: ele organiza tudo para que os programas e o hardware funcionem bem juntos.

- Gerenciamento de Processos: Imagine que você está usando vários programas ao mesmo tempo, como o navegador, um editor de texto e uma música no Spotify. O sistema operacional coordena esses processos, garantindo que todos tenham sua vez de usar o processador sem conflitos. Ele faz isso com um "escalonador", que organiza a fila de execução.

- Gerenciamento de Memória: Já percebeu que, mesmo com muitos programas abertos, eles não se "atrapalham"? Isso acontece porque o SO reserva um espaço específico de memória para cada programa e cuida para que eles não invadam o espaço dos outros.

- Gerenciamento de Dispositivos de Entrada e Saída: Pense nos seus dispositivos, como teclado, mouse e impressora. O SO faz a ponte entre eles e os programas, garantindo que todos funcionem de forma sincronizada. Exemplo: enquanto você digita em um editor de texto, o SO coordena o teclado e a tela para exibir as letras corretamente.

- Gerenciamento de Arquivos: Quando você salva um documento, o sistema operacional organiza esses dados no disco e protege para que ninguém o acesse sem permissão (se você configurar isso). Ele também te ajuda a encontrar arquivos rapidamente, como em uma pesquisa no Explorador de Arquivos.

# Questão 2. Estrutura de sistemas operacionais

## Texto informativo
### Estrutura de Sistemas Operacionais: Custo de Desenvolvimento e Segurança da Informação

A estrutura de um sistema operacional (SO) é fundamental para determinar tanto o custo de desenvolvimento e manutenção quanto a segurança da informação. Existem várias arquiteturas de SO, como monolítica, microkernel e em camadas, cada uma com suas próprias implicações em termos de custo e segurança.

#### Custo de Desenvolvimento e Manutenção

1. **Arquitetura Monolítica**:
   - **Desenvolvimento**: Geralmente, mais rápida de desenvolver inicialmente, pois todos os componentes do SO são integrados em um único bloco de código.
   - **Manutenção**: Pode ser mais complexa e cara, pois qualquer alteração em um componente pode afetar todo o sistema, exigindo testes extensivos e cuidadosos.

2. **Arquitetura Microkernel**:
   - **Desenvolvimento**: Pode ser mais demorada e cara inicialmente, pois envolve a criação de um núcleo mínimo e a implementação de serviços adicionais como processos separados.
   - **Manutenção**: Mais fácil e menos custosa, já que os componentes são isolados. Atualizações e correções podem ser feitas em módulos específicos sem impactar o núcleo do sistema.

3. **Arquitetura em Camadas**:
   - **Desenvolvimento**: Moderadamente complexa, pois cada camada deve ser bem definida e interagir corretamente com as outras.
   - **Manutenção**: Relativamente fácil, pois problemas podem ser isolados e corrigidos em camadas específicas sem afetar o restante do sistema.

#### Segurança da Informação

1. **Arquitetura Monolítica**:
   - **Segurança**: Pode ser mais vulnerável, pois uma falha em qualquer parte do sistema pode comprometer todo o SO. A integração de todos os componentes em um único bloco de código pode dificultar a implementação de medidas de segurança robustas.

2. **Arquitetura Microkernel**:
   - **Segurança**: Geralmente mais segura, pois isola os serviços em processos separados. Isso limita o impacto de uma falha ou ataque a um único componente, protegendo o núcleo do sistema e outros serviços.

3. **Arquitetura em Camadas**:
   - **Segurança**: Oferece um bom equilíbrio, pois cada camada pode implementar suas próprias medidas de segurança. No entanto, a comunicação entre camadas deve ser cuidadosamente gerenciada para evitar vulnerabilidades.

### Conclusão

A escolha da arquitetura de um sistema operacional tem um impacto significativo tanto no custo de desenvolvimento e manutenção quanto na segurança da informação. Arquiteturas monolíticas podem ser mais rápidas e baratas de desenvolver inicialmente, mas podem acarretar custos de manutenção mais altos e maiores riscos de segurança. Por outro lado, arquiteturas microkernel e em camadas podem exigir um investimento inicial maior, mas oferecem vantagens em termos de manutenção e segurança.

## Questão
Com base no texto sobre a estrutura de sistemas operacionais, analise como as diferentes arquiteturas (monolítica, microkernel e camadas) impactam o custo com a equipe de desenvolvimento e a segurança do sistema operacional. Em sua resposta, considere os seguintes pontos:
- Complexidade de implementação e manutenção
- Necessidade de especialização da equipe
- Potenciais vulnerabilidades de segurança
- Facilidade de atualização e correção de falhas

**Dica:** Utilize exemplos de sistemas operacionais reais que adotam essas arquiteturas para ilustrar sua análise.

**Copilot informa**: Essa questão incentiva os alunos a considerarem tanto os aspectos econômicos quanto os de segurança ao avaliar diferentes arquiteturas de sistemas operacionais.

# Questão 2 - Resposta
Sistemas operacionais podem ser construídos de maneiras diferentes, e isso afeta tanto os custos quanto a segurança. 

Arquitetura Monolítica:
Imagine uma caixa cheia de peças misturadas, todas funcionando juntas. Essa é a ideia por trás de sistemas monolíticos, como o UNIX. É mais rápido e barato de construir, mas, se uma peça der problema, o sistema inteiro pode ser afetado. Além disso, consertar qualquer coisa pode ser trabalhoso porque tudo está interligado.

Arquitetura Microkernel:
Agora imagine que cada peça está em uma caixinha separada. Essa é a ideia do microkernel, usado em sistemas como o Minix. É mais seguro, porque, se uma caixinha quebrar, as outras continuam funcionando. No entanto, fazer tudo modular assim dá mais trabalho e custa mais no início.

Arquitetura em Camadas:
Aqui, as peças são organizadas em níveis, como andares de um prédio, com cada andar cuidando de algo específico. Isso facilita a manutenção, pois dá para mexer em um andar sem atrapalhar os outros. Por outro lado, essa organização exige mais planejamento e aumenta a complexidade inicial.

# Questão 3. Introdução à Segurança de Sistemas Operacionais

## Texto informativo

A segurança de um sistema operacional é um aspecto crucial que visa proteger os recursos do sistema contra acessos não autorizados, ataques maliciosos e falhas. Um sistema operacional seguro deve garantir a integridade, confidencialidade e disponibilidade dos dados e serviços. Para alcançar esses objetivos, várias técnicas e mecanismos são implementados, incluindo:

1. **Controle de Acesso**: Define quem pode acessar o sistema e quais recursos podem ser utilizados. Isso é feito através de autenticação (verificação de identidade) e autorização (permissão de acesso).

2. **Criptografia**: Utilizada para proteger dados em trânsito e em repouso, garantindo que apenas usuários autorizados possam acessar informações sensíveis.

3. **Auditoria e Monitoramento**: Registra atividades do sistema para detectar e responder a comportamentos suspeitos ou anômalos.

4. **Isolamento de Processos**: Garante que os processos sejam executados em ambientes isolados, evitando que um processo comprometa a segurança de outro.

5. **Atualizações e Patches**: Manter o sistema operacional atualizado é essencial para corrigir vulnerabilidades conhecidas e proteger contra novas ameaças.


## Questão

Considerando os mecanismos de segurança discutidos, analise como a implementação de controles de acesso e criptografia pode impactar a performance e a usabilidade de um sistema operacional. Em sua resposta, aborde os seguintes pontos:
- Benefícios e desafios de cada mecanismo
- Impacto na experiência do usuário
- Exemplos de situações onde esses mecanismos são críticos

**Dica:** Pense em como esses mecanismos são aplicados em sistemas operacionais que você utiliza no dia a dia, como Windows, Linux ou macOS.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre o equilíbrio entre segurança, performance e usabilidade, aplicando conceitos teóricos a contextos práticos.

# Questão 3 - Resposta
Segurança é um dos pilares de um bom sistema operacional. Dois mecanismos super importantes para isso são o controle de acesso e a criptografia

Controle de Acesso:
É como uma portaria de prédio: só entra quem tem autorização. O sistema verifica quem você é (autenticação) e o que você pode fazer (autorização). Exemplo: quando você coloca a senha para desbloquear seu notebook, está passando por um controle de acesso. O problema é que, se o sistema for muito rigoroso, pode complicar a vida do usuário, pedindo confirmações o tempo todo.

Criptografia:
Um exemplo são os "dados criptografados" que é como colocar suas informações em um cofre, só quem tem a chave pode acessar. Isso protege suas mensagens e arquivos de olhos curiosos. Exemplo: ao fazer uma compra online, a criptografia garante que seus dados do cartão fiquem seguros. O desafio aqui é que ela pode deixar o sistema mais lento, especialmente em máquinas menos potentes.

# Questão 4. Custo de Processamento versus Algoritmo Ótimo de Escalonamento

## Texto informativo

O escalonamento de processos é uma função crítica de um sistema operacional, responsável por determinar a ordem em que os processos são executados pelo processador. O objetivo é maximizar a eficiência do sistema, garantindo que os recursos sejam utilizados de maneira justa e eficaz. No entanto, encontrar o algoritmo de escalonamento ótimo envolve um equilíbrio delicado entre o custo de processamento e a eficiência do escalonamento.

### Custo de Processamento

O custo de processamento refere-se ao tempo e aos recursos necessários para executar um algoritmo de escalonamento. Algoritmos mais complexos podem oferecer melhores resultados em termos de tempo de resposta e utilização do processador, mas também podem exigir mais recursos computacionais para tomar decisões de escalonamento. Isso pode incluir tempo de CPU, memória e outras operações de sistema.

### Algoritmo Ótimo de Escalonamento

Um algoritmo ótimo de escalonamento é aquele que maximiza a eficiência do sistema operacional, minimizando o tempo de espera dos processos, o tempo de resposta e o tempo de retorno. Alguns dos algoritmos de escalonamento mais comuns incluem:

- **First-Come, First-Served (FCFS)**: Simples e fácil de implementar, mas pode levar a longos tempos de espera para processos curtos.
- **Shortest Job Next (SJN)**: Minimiza o tempo médio de espera, mas pode ser difícil de implementar devido à necessidade de prever o tempo de execução dos processos.
- **Round Robin (RR)**: Oferece uma abordagem justa, atribuindo fatias de tempo iguais a todos os processos, mas pode resultar em maior sobrecarga de contexto.
- **Priority Scheduling**: Processos com maior prioridade são executados primeiro, mas pode levar à inanição de processos de baixa prioridade.

## Questão

Considerando os conceitos de custo de processamento e algoritmo ótimo de escalonamento, analise como diferentes algoritmos de escalonamento podem impactar a performance de um sistema operacional em termos de tempo de resposta, tempo de espera e utilização do processador. Em sua resposta, aborde os seguintes pontos:
- Vantagens e desvantagens de pelo menos dois algoritmos de escalonamento
- Impacto do custo de processamento na escolha do algoritmo
- Exemplos de situações onde um algoritmo pode ser preferível a outro

**Dica:** Pense em como esses algoritmos são aplicados em diferentes cenários, como sistemas de tempo real, servidores web e sistemas operacionais de uso geral.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre a complexidade e os trade-offs envolvidos na escolha de um algoritmo de escalonamento, aplicando conceitos teóricos a contextos práticos.

# Questão 4 - Respostas
Imagine que você está organizando uma fila de pessoas para usar um único caixa eletrônico. Essa fila é como os processos no computador, e o "algoritmo de escalonamento" é o método usado para decidir quem será atendido primeiro. Aqui vão dois exemplos:

First-Come, First-Served (FCFS):
Esse é simples: quem chega primeiro, é atendido primeiro. É fácil de implementar, mas pode ser injusto. Imagine que alguém na frente da fila demora muito; todos atrás terão que esperar, mesmo que suas tarefas sejam rápidas.

Round Robin (RR):
Aqui, todos têm uma chance de usar o caixa por um tempo limitado, e depois vão para o fim da fila. É justo, mas tem um custo extra de reorganizar a fila o tempo todo, o que pode atrasar o processo.

Cada algoritmo tem suas vantagens e desvantagens, e a escolha se baseia em: justiça, eficiência ou simplicidade. Por exemplo, em jogos online, é essencial garantir respostas rápidas (tempo real), então um algoritmo diferente seria escolhido.

# Questão 5. Aplicativo em python vs aplicativos em c

## Questão

Explique o caminho que as instruções seguem desde um aplicativo escrito em Python e um aplicativo escrito em linguagem C até serem executadas pelo hardware. Em sua resposta, considere os seguintes pontos:
- O papel do interpretador no caso do Python
- O processo de compilação no caso do C
- A interação entre o kernel do sistema operacional e os drivers de dispositivo
- A tradução final das instruções para o formato binário (0 e 1) executado pelo hardware

**Dica:** Compare e contraste os dois processos, destacando as principais diferenças e semelhanças na forma como as instruções são processadas e executadas.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre os diferentes caminhos que as instruções seguem em linguagens interpretadas e compiladas, aplicando conceitos teóricos a contextos práticos.

# Questão 5 - Respostas
As linguagens Python e C seguem caminhos diferentes.

Python:
O código é interpretado "ao vivo" pelo interpretador Python. Ele pega as instruções do seu programa e as traduz para algo que o computador entende, mas faz isso enquanto o programa está rodando. Por isso, é mais fácil escrever e corrigir, mas pode ser mais lento.

C:
O código é transformado (compilado) em um arquivo executável antes de ser usado. Esse arquivo já está no "idioma" do computador, então ele roda de forma muito mais eficiente. Por outro lado, fazer mudanças no programa exige recompilar tudo.

Ambas as linguagens interagem com o sistema operacional e, no fim, tudo vira binário (0s e 1s) para o hardware executar. Python é ótimo para protótipos e scripts rápidos, enquanto C brilha em sistemas onde cada milissegundo conta, como dispositivos embarcados.
