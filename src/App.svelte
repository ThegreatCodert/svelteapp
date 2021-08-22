<script>
	 
	 let result = " " ; 
	function rockButton() {
		let randomNumber = Math.floor(Math.random() * 3);
		
		if (randomNumber == 1) {
			result =  "You lost😭";
		} else if (randomNumber == 2) {
			result =  "You won😀";
		} else if (randomNumber == 0) {
			result = "Tie🙂";
		}
	}

	function paperButton() {
		let randomNumber = Math.floor(Math.random() * 3);
		if (randomNumber == 1) {
			result =  "Tie🙂";
		} else if (randomNumber == 2) {
			result = "You lost😭";
		} else if (randomNumber == 0) {
			result = "You won😀";
		}
	}

	function scissorButton() {
		let randomNumber = Math.floor(Math.random() * 3);
		if (randomNumber == 1) {
			result = "You won😀";
		} else if (randomNumber == 2) {
			result = "You Tie🙂";
		} else if (randomNumber == 0) {
			cresult =  "You lost😭";
		}
	}

	 
</script>
<body>
	<div id="above">
		Rock Paper and Scissors
	</div>
	
	<div id="color">
		<button class = "rock"on:click={rockButton}><i class="fa fa-hand-rock-o" aria-hidden="true"></i></button>
		<button class = "paper" on:click={paperButton}><i class="fa fa-hand-paper-o" aria-hidden="true"></i></button>
		<button on:click={scissorButton}><i class="fa fa-hand-scissors-o" aria-hidden="true"></i></button>
	</div>
	<div id="resultss"><h3>{result}</h3></div>
	
</body>

<style>
	body{
		background-color: #24272E;
	}
	 #above{
		padding: 10px;
	 }
	 #color{
		 /* background-color: purple; */
		 padding: 3%;
	 }
	 #resultss{
		position: absolute;
  		top: 50%;
  		left: 50%;
  		transform: translate(-50%, -50%);
		border: 3px;
    	border-color: whitesmoke;
    	border-style: solid;
		width: 50%;
		height:25%
	 }
</style>
 
