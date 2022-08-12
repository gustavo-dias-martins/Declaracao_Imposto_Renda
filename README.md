<h1> Automatização do Preenchimento do Imposto de Renda </h1>
<p>Quem nunca perdeu dias declarando o imposto de renda? Sempre fazendo o mesmo processo repetitivo coletando as informações em folhas/planilhas avulsas e preenchendo no imposto de renda com o mesmo padrão só trocando algumas informações.</p> 
<p>O projeto é um código desenvolvido em Python, desenvolvido no Jupyter para automatizar esse preenchimento e reduzir o tempo que levamos nesse processo.</p>

<h2> Bibliotecas Utilizadas </h2>
<p>- Pyautogui</p>
<p>- Pyperclip</p>
<p>- Time</p>
<p>- Pathlib</p>
<p>- Pandas</p>

<h2> Arquivos Utilizados </h2>
<h3> Pasta Bases: </h3>
<p>- B3_2021 -> Base extraída do site da B3 com todas operações realizadas. Com o passar do tempo essa base aumenta pois iremos juntando as operações de cada ano em uma tabela única.</p>
<p>- Importar_Dados -> As informações recebidas dos bancos e corretoras que são essenciais para a declaração</p>
<p>- Informações_FIIS_Ações -> Informações dos Fundos Imobiliários e Ações, como Razão Social e CNPJ que retiramos do site da B3</p>
<p>- Renda Variável -> Arquivo que nosso código terá gerado ao declararmos no ano anterior com as informações de valor total declarado e sua preço médio ponderado por ticker. </p>
<h3> Pasta Imagens: </h3>
<p>- Bens e Direitos</p>
<p>- Estados Unidos</p>
<p>- Rendimentos não Tributáveis</p>
<p>- Rendimentos Tributação Exclusiva</p>


<h2> Como funciona? </h2>
<p>Em vez de cada etapa do preenchimento do imposto buscarmos as indormações em folhas/planilhas distintas, nesse primeiro momento focamos em juntar todas as informações necessáris em um único lugar (arquivo Importar_Dados).</p> 
<p>Após essa estapa nosso código irá calcular, utilizando o Pandas, a média ponderada dos preços de cada ticker comprado e vendido, para que no final possamos declarar quanto de patrimônico temos em cada ticker.</p>
<p>Utilizaremos o Pyautogui e o Pyperclip para preencher as informações no programa da Receita Federal que teremos baixado. Em alguns pontos dos códigos, ele utiliza imagens, que estão na pasta "Imagens" para clicar no ponto desejado.</p>
<p>O projeto <b>não é para preencher todo o imposto de renda</b>, foi desenvolvido para simplicar nosso trabalho. Exemplos do que ele preenche:</p>
<p>- Bens e Direiro</p>
<p>- Redimentos não Tributáveis</p>
<p>- Rendimentos Tributação exclusiva</p>
<p>- Investimento nos Estados Unidos</p>

https://user-images.githubusercontent.com/104008210/184379255-eac09b2f-330b-42eb-a40e-1c2bc6153142.mov

