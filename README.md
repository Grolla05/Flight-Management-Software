<h1>Relatório de Projeto – Flight Management Software</h1>

<p><strong>Disciplina:</strong> Programação<br>
<strong>Instituição:</strong> Pontifícia Universidade Católica de Campinas – Escola Politécnica<br>
<strong>Curso:</strong> Engenharia de Computação</p>

<p><strong>Autores:</strong><br>
- Felipe Cassante Ganzarolli — RA: 24003492<br>
- Felipe Grolla Freitas — RA: 24004846<br>
- Gabriel Henrique Pozeti de Faria — RA: 24011960<br>
- João Victor Vasconcelos Junqueira Criscuolo — RA: 22024547<br>
- Lucas Espica Rezende — RA: 24006575</p>

<p><strong>Campinas — SP</strong><br>
<strong>Ano:</strong> 2024</p>

<h2>1. Introdução</h2>
<p>O presente relatório tem como objetivo apresentar o processo de desenvolvimento de um software, criado na linguagem C, voltado para a gestão de voos de uma companhia aérea fictícia denominada <strong>“Voe Sempre, Voe Feliz”</strong>, bem como os resultados obtidos ao longo do projeto.</p>
<p>O sistema desenvolvido busca oferecer funcionalidades essenciais para o gerenciamento eficiente de voos, como a adição, alteração e exclusão de voos, bem como filtros de busca baseados nos voos cadastrados.</p>
<p>Através da implementação dessas funcionalidades, o sistema visa otimizar o processo de administração dos itinerários, garantindo a precisão das informações disponibilizadas aos usuários e promovendo maior eficiência operacional para a companhia aérea.</p>

<h2>2. Proposta de Projeto e Desenvolvimento</h2>

<h3>2.1. Menu de Início</h3>
<p>O sistema desenvolvido apresenta, em sua tela inicial, um menu (função <code>main</code>) que permite ao usuário escolher e selecionar uma das oito funcionalidades disponíveis:</p>
<ul>
  <li>Incluir voo</li>
  <li>Alterar informações de um voo</li>
  <li>Excluir um voo</li>
  <li>Determinar quais voos saem de uma cidade de origem escolhida</li>
  <li>Determinar qual voo, entre os que saem e chegam em cidades iguais, possui o menor número de escalas</li>
  <li>Determinar quais voos chegam a uma cidade de destino escolhida</li>
  <li>Exibir todos os voos e suas informações</li>
  <li>Sair do sistema</li>
</ul>
<p>Ao final de cada função (exceto a última), o menu é apresentado novamente ao usuário. Além disso, em qualquer função, o usuário pode digitar “-1” a qualquer momento para encerrar a operação prematuramente.</p>

<h3>2.2. Função 1 – Incluir Voo</h3>
<p>Adiciona novos voos ao sistema. O sistema verifica voos duplicados, solicita informações do voo (com conversão para letras maiúsculas), confirma dados e repete o processo conforme o desejo do usuário. Ao final, atualiza o contador de voos e controla o limite máximo.</p>

<h3>2.3. Função 2 – Alterar Informações de um Voo</h3>
<p>Permite modificar os dados de voos já cadastrados. Inclui a edição de escalas, remoção ou troca de cidades de escala. Verifica entradas inválidas e apresenta mensagens de erro. Se não houver voos cadastrados, pausa a execução e informa o usuário.</p>

<h3>2.4. Função 3 – Apagar Voo</h3>
<p>Exclui voos cadastrados após validação do número do voo. Reorganiza o vetor de voos e atualiza o contador. Se não houver voos, exibe erro e retorna ao menu principal.</p>

<h3>2.5. Função 4 – Determinar Quais Voos Saem de uma Cidade de Origem Escolhida</h3>
<p>Filtra voos com base na cidade de origem inserida pelo usuário. Exibe os resultados ou, em caso de inexistência, informa o usuário. Converte entradas para maiúsculo e pausa execução para leitura da mensagem.</p>

<h3>2.6. Função 5 – Determinar Qual Voo Dentre Todos os que Saem e Chegam em Cidades Iguais Possui o Menor Número de Escalas</h3>
<p>Lista todos os voos e identifica o voo com menor número de escalas entre cidades especificadas pelo usuário. Verifica se há voos e informa caso contrário. Converte cidades para letras maiúsculas para comparação.</p>

<h3>2.7. Função 6 – Determinar Quais Voos Chegam em uma Cidade de Destino Escolhida</h3>
<p>Filtra os voos com destino à cidade especificada. Mostra todos os dados relacionados ou informa que não há voos disponíveis. Pausa a execução ao final para permitir leitura da mensagem.</p>

<h3>2.8. Função 7 – Exibir Todos os Voos e suas Informações</h3>
<p>Exibe todos os voos cadastrados no sistema, com seus respectivos dados (incluindo escalas). Caso não haja voos, limpa a tela e exibe mensagem solicitando adição de voos.</p>

<h3>2.9. Função 8 – Sair do Programa</h3>
<p>Permite ao usuário encerrar o programa. Utiliza o comando <code>exit(0)</code> na função <code>main</code> para encerramento imediato.</p>

<h2>3. Dificuldades, Soluções e Desenvolvimento do Projeto</h2>
<p>Entre os principais desafios enfrentados pelo grupo, destacam-se:</p>
<ul>
  <li>Compreensão e manipulação de ponteiros;</li>
  <li>Impressão adequada de todas as escalas e cidades correspondentes;</li>
  <li>Uso de estruturas <code>switch-case</code> aninhadas;</li>
  <li>Padronização de nomes de variáveis e comunicação entre os membros;</li>
  <li>Necessidade de uso do <code>fflush</code> para controle de buffer.</li>
</ul>
<p>Tais dificuldades foram superadas com aprofundamento em estudos teóricos e práticos sobre os conceitos envolvidos. Quando necessário, o grupo buscou auxílio da professora da disciplina, que forneceu orientações adequadas.</p>

<h2>4. Conclusão</h2>
<p>O desenvolvimento do sistema de gerenciamento de voos atingiu os objetivos propostos, entregando uma plataforma funcional e eficiente.</p>
<p>As funcionalidades implementadas — como adição, edição e exclusão de voos, filtros e listagens — demonstraram eficiência na simulação de processos reais de uma companhia aérea.</p>
<p>O uso da linguagem C permitiu criar uma aplicação robusta, com possibilidade de expansão. O projeto comprovou sua viabilidade técnica e reforçou a importância do gerenciamento de dados no setor aéreo.</p>

<h2>5. Referências</h2>
<p>GUIMARÃES, Lúcia Filomena de Almeida. <i>SEGUNDO_PROJETO-1.docx</i>, 2024.<br>
Disponível em: <a href="https://puc-campinas.instructure.com/courses/51258/files/2423775?wrap=1" target="_blank">https://puc-campinas.instructure.com/courses/51258/files/2423775?wrap=1</a><br>
Acesso em: 21 de maio de 2024.</p>
