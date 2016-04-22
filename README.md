<!DOCTYPE html>
<html>
    <head> 
    <h1>JavaScript Can Validate Input</h1>
    <p>please input a number between 1 and 10</p>
    <input id='numb'>
    <button type='button' onclick="myFunction">Submit</button>
    <p id='demo'></p>
    <script>
        function myFunction() {
            var x, text;
            //Get The value of the input field with id="numb"
            x = document.getElementById("numb").value;

            //if x is Not a Number or less than one or greather than 10
            if (isNaN(x) || x < 1 || x > 10) {
                text = "input not valid";
            } else {
                text = "input OK";
            }
            document.getElementById("demo").innerHTML = text;
        }
    </Script>
</head>
</html>
