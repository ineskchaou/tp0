# tp0
<!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>


<h3><center>JavaScript Click Counter</center></h3>
<center>
<div>
	<button onclick="incrementClick()"> Cliquez-Moi pour compter</button>
</div>
<div>
    <center><h3 id="counter-label">0</h3></center>
</div>

    <div>
        
        <button onclick="resetCounter()">Remettre le compteur à 0</button>
    </div>
</center>
<script type="text/javascript">
var counterVal = 0;

function incrementClick() {
    updateDisplay(++counterVal);
}

function resetCounter() {
    counterVal = 0;
    updateDisplay(counterVal);
}

function updateDisplay(val) {
    document.getElementById("counter-label").innerHTML = val;
}
</script>
</body>
</html>
