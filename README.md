# InvertCadena
#Funcion que Invierte una cadena de caracteres
<HTML>
<HEAD>
<SCRIPT>
 
function revWord(str){
	var x = str.length; 
	var backWord = " ";  
	while (x>=0) {
	 backWord = backWord + str.charAt(x);
        x--
      }
	 document.theForm.results.value = backWord;
}
</SCRIPT>
</HEAD>
<BODY>
<FORM name="theForm">
Introduzca una Palabra:
<TEXTAREA name=inStr rows=5 cols=90>
</TEXTAREA>
<INPUT type=button value="Palabra invertida" onClick="revWord(document.theForm.inStr.value)";>
<INPUT type=button name="theButton" value="Limpiar Resultado" onClick='document.theForm.results.value=""';>
Resultado<br>
<TEXTAREA name=results rows=5 cols=90>
</TEXTAREA>
</FORM>  
</BODY>
</HTML>
