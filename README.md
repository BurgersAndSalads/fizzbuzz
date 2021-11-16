# fizzbuzz

Click on the start button to see a list of numbers, from 1 to 100

If the number is divisible by 3, then fizz will appear

If the number is divisible by 5, then buzz will appear

If the number is divisible by both, then fizz buzz will appear

have fun

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>9thCO technical task</title>
</head>
<body>

    <!-- 
        16. In an HTML file, create a function using JavaScript that will insert the numbers 1 to 100 into an unordered list. 
        Where the number is a multiple of 3, append ‘Fizz’, otherwise if it is a multiple of 5 append ‘Buzz’.
        Style the page and have this function trigger when a user clicks a button with the text start.
        Bonus: upload the file to a repository with a Readme outlining the application.
    -->

    <button onclick="fizzBuzz()">Start</button>
    <ul id="fizzBuzz"></ul>
    <script>
        function fizzBuzz() 
        {
            const list = document.getElementById('fizzBuzz');
            for(let i = 1; i <= 100; i++) 
            {
                let createItems = document.createElement('li');
                createItems.setAttribute('id', i);
                let append = " ";
                if (i % 3 === 0)
                {
                    append += 'Fizz';
                } 
                if (i % 5 === 0)
                {
                    append += 'Buzz';
                }
                createItems.innerHTML = i + append;
                list.appendChild(createItems);
            }
        }
    </script>

    
</body>
</html>
