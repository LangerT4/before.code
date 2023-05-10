<!DOCTYPE html>
<html>
<head>
	<title>Random Quote Example</title>
	<style>
		h1 {
			font-size: 24px;
			text-align: center;
		}
	</style>
</head>
<body>
	<h1 id="random-quote"></h1>
	<button onclick="generateQuote()">Generate Quote</button>
	<script>
		// Define an array of quotes
		var quotes = [
			"The best way to predict your future is to create it. - Abraham Lincoln",
			"The only way to do great work is to love what you do. - Steve Jobs",
			"Believe you can and you're halfway there. - Theodore Roosevelt",
			"Don't watch the clock; do what it does. Keep going. - Sam Levenson",
			"The greatest glory in living lies not in never falling, but in rising every time we fall. - Nelson Mandela"
		];

		// Define a function to generate a random quote
		function generateQuote() {
			// Get a random quote from the quotes array
			var randomIndex = Math.floor(Math.random() * quotes.length);
			var randomQuote = quotes[randomIndex];

			// Update the text of the h1 element with the random quote
			var quoteElement = document.getElementById("random-quote");
			quoteElement.innerHTML = randomQuote;
		}
	</script>
</body>
</html>
