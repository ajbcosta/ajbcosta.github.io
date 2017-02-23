<html>

<head>
<title>A minha primeira página Web</title>

</head>

<body>

<h1>Esta é a minha primeira página de HTML</h1>
<h5>Criada com base no curso de Web Development da <a href="https://alison.com/topic/learn/1255/24414/html-coding-create-web-pages/">Alison.com</a></h5>
<hr>
<a name="início">
<h3><font color="blue">Notas sobre este curso:</font></h3>

<p>1) neste momento está página está num ficheiro (html) no meu computador, mas o que se pretende é que este ficheiro seja carregado num servidor web (Web Server)</p>
<p>2) um <b>Web Server</b> é um computador desenhado para estar sempre ligado à internet e assim poder ser acedido em qualquer parte do mundo</p>
<p>3) com o ficheiro (html) carregado no Web Server, alguém com o endereço da página pode descarregá-lo para o seu computador, através de um Web Browser, e ver o documento</p>
<p>4) o <b>título da página</b> está identificado na "cabeça" do documento (com a tag &lt;title&gt;) e é importante para as pesquisas feitas através de um motor de pesquiza, é o nome que aparece na listagem</p>
<p>5) <b>entidades</b> são uma forma de adicionar caracteres especiais que não seriam permitidos de outra forma, começam por “&” e terminam com “;”, para consultar a lista basta googlar "html entities"</p>
<p>6) <b>links</b> para outras páginas são indicados através de etiquetas âncora (anchor tags): &lt;a&gt;link&lt;&#47;a&gt;</p>
<p>7) <b>atributo</b> é algo que se adiciona a uma tag para adicionar informação à cerca dela. Por exemplo para um link utiliza-se o atributo "href": &lt;a&nbsp;href="nome da página"&gt;link&lt;&#47;a&gt;</p>
<p>8) link para outra página: <a href="02teste.html">link</a> de exemplo</p>
<p>9) o link anterior é um <b>link relativo</b> (relativo à pagina em que se está), por exemplo <a href="teste\03teste.html" target="_blank">este</a> aponta para uma página que está numa subpasta e é aberto numa nova tab do browser</p>
<p>10) ao contrário de um <b>link absoluto</b>, onde é dado o caminho completo, como neste <a href="D:\SkyDrive\10. MyProject\93. Página Web\01.PáginaTeste\03teste.html">exemplo</a>. Este tipo de links são de evitar pois ficam presos a uma estrutura que pode mudar ao longo do tempo</p>
<p>11) para incluir <b>imagens</b> a tag é &lt;img&nbsp;src="caminho (relativo) e nome da imagem "&gt;</p>
<p></p>
<p>
<center><img src="imagens\conan.BMP"></center>
</p>
<p>
<center>(no tamanho original)</center>
</p>
<p>12) para alterar o tamanho da imagem há que adicionar os atributos "height" e "width" (ou apenas um deles e o browser determina o outro através do rácio da foto)</p>
<p>
<center><img src="imagens\conan.BMP" height="100" title="a foto do Conan"></center>
</p>
<p>13) aumentado o tamanho para além do original o browser tenta adivinhar a informação em falta, o melhor mesmo é trabalhar as imagens num editor próprio e utilizar as imagens no seu tamanho original</p>
<p>14) idealmente a edição de html, deverá ser feita num programa próprio (em vez de notepad simples) pois facilita a leitura e o desenvolvimento, com o fecho automático de tags e ajudando com os atributos e valores possíveis de cada um</p>
<p>&nbsp;&nbsp;&nbsp;i) <a href="https://www.adobe.com/pt/products/dreamweaver.html">Dreamweaver (muito bom mas pago)</a></p>
<p>&nbsp;&nbsp;&nbsp;ii) <a href="https://www.microsoft.com/en-us/download/details.aspx?id=36179&ranMID=24542&ranEAID=TnL5HPStwNw&ranSiteID=TnL5HPStwNw-Zr71mcRYJenbGOJnjYbTdw&tduid=(b41c67d2e6f2082dd4d7645d1a95c16d)(256380)(2459594)(TnL5HPStwNw-Zr71mcRYJenbGOJnjYbTdw)()">Microsoft Expression Web 4 (Free Version)</a></p>
<p>&nbsp;&nbsp;&nbsp;iii) <a href="https://www.activestate.com/komodo-ide/downloads/edit">Komodo Edit</a></p>
<p>&nbsp;&nbsp;&nbsp;iv) <a href="https://html-online.com/">Editor online free</a></p>
<p>15) tags de apresentação básica como a fonte, cor, sublinhado, itálico, negrito, etc... outras formas de apresentação serão faladas no âmbito do CCS mais adiante</p>
<p>&nbsp;&nbsp;&nbsp;i) <font color="blue">cor azul</font> ou uma cor <font size="15" color="#45828D">azulada em grande</font> para saber o código de uma cor utilizar por exemplo esta <a href="http://paletton.com">palete</a> online</p>
<p>&nbsp;&nbsp;&nbsp;ii) <b>negrito (bold) e <i>itálico</i> e <u>sublinhado (underline)</u></b> e <br> numa nova linha</p>
<p>&nbsp;&nbsp;&nbsp;iii) linha</p>
<hr>
<p>&nbsp;&nbsp;&nbsp;iv) linha de uma tamanho específico</p>
<hr width="100px">
<p></p>
<p>16) para criar links dentro da própria página, basta criar uma tag de "ancoragem" na própria página. Por exemplo para ir para o <a href="#início">início</a></p>
<p>17) para criar links para um local específico dentro de outra página, basta criar uma tag de "ancoragem" nessa página e referênciar como &lt;a href="nome da pagina#nome da tag"&gt;</p>
<p>18) para criar tabelas</p>
<p>&nbsp;&nbsp;&nbsp;i) "tr" = table row; "th" = table header; "td" = table data</p>

<table border="1" width="600px" align="center"><!--há vários atributos: cor,largura das linhas, etc, etc...-->
<caption align="bottom">Tabela de teste</caption>
	<tr>
		<th width=200px">Cabeçalho 1</th>
		<th>Cabeçalho 2</th>
		<th>Cabeçalho 3</th>
		<th>Cabeçalho 4</th>
	</tr>
	<tr>
		<td rowspan=2><!--Para fazer o merge de linhas-->
			<table border="1"><!--tabela dentro de uma tabela-->
				<tr>
					<th>mini1</th>
					<th>mini2</th>
				</tr>
				<tr>
					<td>1</td>
					<td>2</td>
				</tr>
			</table>
		</td>
		<td colspan=2 align="center" valign="center">(1,2)</td><!--Para fazer o merge de colunas-->
		<td>(1,3)</td>
	</tr>
	<tr>
		<td>(2,2)</td>
		<td>(2,3)</td>
		<td>(2,4)</td>
	</tr>
</table>
<p>&nbsp;&nbsp;&nbsp;ii) este tipo de tabelas não parece ser muito utilizado, mas na realidade são, ver por exemplo este <a href="http://www.bbc.com/" target="_blank">site</a> (e com as opções de programador fazer o outline das tabelas)</p>
<p>19) <b>listas</b> podem ser: ordenadas; desordenadas; (de) definição</p>
<p>&nbsp;&nbsp;&nbsp;i) Ordenadas</p>
<ol><!--ordered list-->
	<li>Item 1</li><!--list item-->
	<li>Item 2</li>
	<li>Item 3</li>
</ol>
<p>&nbsp;&nbsp;&nbsp;ii) Desordenadas</p>
<ul><!--unordered list-->
	<li>Item 1</li>
	<li>Item 2</li>
	<li>Item 3</li>
</ul>
<p>&nbsp;&nbsp;&nbsp;iii) Definição</p>
<dl><!--definition list-->
	<dt>termo 1</dt><!--definition term-->
	<dd>definição do termo 1</dd><!--definition detail-->
	<dt>termo 2</dt>
	<dd>definição do termo 2</dd>
</dl>
<p>20) carregar a página num servidor web</p>
<p>&nbsp;&nbsp;&nbsp;1. primeiro é necessário um espaço na web (web space) fornecido pelo ISP ou através de web hosting sites</p>
<p>&nbsp;&nbsp;&nbsp;2. segundo será necessário um programa de <b>ftp</b> para transferir o ficheiro html do computador para o servidor web (exemplos: <a href="https://winscp.net/eng/download.php">WinSCP</a>; <a href="https://aceftp-free.en.softonic.com">AceFTP</a>)</p>
<p></p>
<p></p>
<p>&nbsp;</p>
<hr>
<p>&copy; copyright António Costa</p>

</body>

</html>

