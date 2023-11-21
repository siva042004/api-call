# JavaScript---9---API-Call-using-fetch
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cat Facts</title>
</head>
<body>

    <div id="cat-fact-container">
        <button onclick="getCatFact()">Get Cat Fact</button>
        <p id="cat-fact"></p>
    </div>

    <script>
        function getCatFact() {

            fetch('https://catfact.ninja/fact')
                .then(response => response.json())
                .then(data => {

                    document.getElementById('cat-fact').textContent = data.fact;
                })
                .catch(error => {
                    console.error('Error fetching cat fact:', error);
                });
        }
        
    </script>
</body>
</html>

```
# output
![Screenshot (81)](https://github.com/21002624/JavaScript---9---API-Call-using-fetch-/assets/113762183/99bf1c42-d115-4e30-98c4-c90c33699952)

