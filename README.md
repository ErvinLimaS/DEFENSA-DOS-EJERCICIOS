# DEFENSA-DOS-EJERCICIOS

<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>Defensa</title>
</head>
<body>
<h1>Ejercicio 7</h1>
<p>Ingrese el valor de n:</p>
<input type="number" id="nInput" value="1000000">
<button onclick="calculateHarmonicSquaredSeries()">Calcular</button>
<p id="result"></p>


<script>
	function calculateHarmonicSquaredSeries() { 
		let n = document.getElementById("nInput").value;
		n = parseInt(n);
		const vector = Array.from({ lenght: n }, (_, i) => 1 / ((i + 1) ** 2));
		const sum = vector.reduce((accumulator, term) => accumulator + term, 0);
		document.getElementById("result").innerHTML = "El resultado es: " + sum.toFixed(4);
	}
</script>


<h1>Ejercicio 8</h1>

<form> <label for="a">Valor de n:</label> <input type="number" id="a" name="ab" value="0"
	> <button type="but" onclick="calculatesum()">Calcular Suma</button> </form> <p>La
		suma para n = <span id="nValue">0</span> es: <span id="result"></span></p> 
		<script> 
			function calculatesum() { let n = document.getElementById("n").value; let sum = 0;
			for (let i = 0; <= n; i++) { sum += 1 / ((2 * i + 1) * (2 * i + 2)); } document.getElementById("nValue").textContent = n; document.getElementById("result").textContent = sum.toFixed(4); }
		</script>
</body>
</html>



CODIGO OCTAVE

EJERCICIO 7

n=input('Ingrese el valor de n, n= ')
s=0;
rf=0;
for i=1:n
i;
s=s+1/i^2;
r=s;
rf=rf+s;
f=rf;
endfor

rf=s;
disp(s)



EJERCICIO 8

function result = harmonic_squared_series()
sum=0;
n=0;
while true
term = 1 / ((2*n+1)*(2*n+2));
sum += term;
n +=1;
if n > 1000000
break;
endif
endwhile
result = sum;
endfunction
