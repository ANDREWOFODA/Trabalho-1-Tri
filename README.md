<!DOCTYPE html>
<html lang="pt-br">
	<head>
		<meta charset="utf-8">
		<title>Calculadora</title>		
		<script src="calculadora.js"></script>
	</head>
	<body bgcolor="beige">
		<h1>Calculadora 1.0</h1>
		<input type="text" id="txtValor1">
			<select id="operadores" onchange="ControleDeSelecao();">
				<optgroup label="Basico">
					<option value="+">	+(somar)</option>
					<option value="-">	-(subtrair)</option>
					<option value="*">	*(multiplicar)</option>
					<option value="/">	/(dividir)</option>
				</optgroup>
				<optgroup label="Outros">
					<option value="raiz">	 	  Raiz	</option>
					<option value="potencia">	Potência</option>
					<option value="fatorial">	Fatorial</option>
					<option value="fibonacci">Fibonaci</option>					
					<option value="porcento">	Porcentagem</option>
					<option value="media">		Média</option>
					<option value="calc">		  Develop Calc</option>
				</optgroup>
			</select>
		<input type="text" id="txtValor2" size="5"><br>		
		<input type="button" onclick="Calcular('txtValor1', 'txtValor2')" value="Calcular">
		<input type="button" onclick="Limpar('txtValor1', 'txtValor2')" value="Limpar">
		<p id="saida">Resultado:</p>
		<hr>		
	</body>
</html>
