# Meus-estudos-em-Java-script-
Comandos mas usados em Java script 
1.Simples função de alerta

<script language="javascript">
function mensagem() {
window.alert("Você clicou neste campo");
}
</script>


<a href="" OnClick="mensagem()">Link comum</a>
2.mudando de cor ao clicar em cima de uma célula da tabela

<script language="javascript">
function cor(celula){
celula = document.getElementById("celula1");
celula.style.backgroundColor="#66ff33"
}
</script>




<table border="1" cellpadding="20">
<tr>
<td id="celula1" onclick="cor()">Nome da Célula
</td>
</tr>
</table>
3.Janela de Confirmação

<script language="JavaScript">
function confirmBox() {
if (confirm("Voce deseja mesmo ir para o Site do Google?")) {
location.href="http://google.com";}
}
</script>


</p><form>
Clique no Botão abaixo para ir para o Site do Google:
<input value="Clique aqui para abri o site do Google" onclick="confirmBox()" type="button">
</form>
4.Alertas em sequencia em botão simples

<form>
<input type="button" Value=" Alerta " onClick="alert('Esta é uma mensagem gerada a partir do clique em um botão de alerta');alert('Aqui temos a segunda mensagem gerada pela segunda janela');alert('Uma terceira mensagem!')")>
</form>
5.alerta ao passar o mouse em cima de imagem ou frase

<a href="" onmouseover = "alert('Esta é uma mensagem gerada pelo recurso OnMouseOver em uma frase.')")><img src="endereço_da_imagem" border="0" width="14" height="14"/>Passe o cursor em cima desta frase.</a>
6.Mensagem de alerta customizada pelo usuário

<form>
<textarea name="text" rows="3" cols="30"></textarea>
<p>
<input value="Alerta Teste!" onclick="alert(this.form.text.value)"
type="button">
<input name="cancel" value="Apague" type="reset">
</form>
7.Janela de alerta após o carregamento completo da página

<body onLoad="window.alert('A tag body foi carregada')">
8.Abrir uma nova janela

<input value="Abrir Janela" onclick="window.open('ENDEREÇO_WEB_OU_LOCAL.html',
'Exemplo',
'toolbar=no,location=no,directories=no,status=no,menubar=no,scrollbars=no,resizable=no,copyhistory=yes,width=300,height=150')"
type="button">
</form>
9.Janela de PROMPT

<script language="JavaScript" TYPE="text/javascript">
var nome;
do {
nome = prompt ("Qual é o seu nome?");
} while (nome == null || nome == "");
alert ("Seu nome é "+nome);
</script>
10.Bloquear botão direito do mouse

<script>
function click() {
if (event.button==2||event.button==3) {
oncontextmenu='return false';
&nbsp; }
}
document.onmousedown=click
document.oncontextmenu = new Function("return false;")
</script>
11.Imprimir a página

<input type="button" value="Imprima"
