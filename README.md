<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Percentage Calculator</title>
</head>
<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: Arial, Helvetica, sans-serif;
    }

    body {
        background-color: #e0e0e0;

    }

    .container {
        background-color: #fff;
        border-radius: 10px;
        width: 90%;
        margin: 10px auto;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    .heading {
        background-color: lightgray;
        text-align: center;
        width: 100%;
        padding: 20px;
        font-size: 20px;
        font-weight: 500;
        margin-bottom: 30px;
        word-spacing: 2px;
        letter-spacing: 2px;
        border-top-left-radius: 10px;
        border-top-right-radius: 10px;
    }

    input {
        padding: 10px;
        width: 15rem;
        margin: 10px auto;
        border: 1px solid lightgrey;
        border-radius: 5px;
    }

    input:focus {
        outline: none;
    }

    p {
        background-color: whitesmoke;
        display: block;
        width: 90%;
        text-align: center;
        font-weight: 600;
        font-size: 18px;
        padding: 5px;
        border: 1px solid lightgrey;
        border-radius: 9px;
    }

    button {
        padding: 6px;
        border: none;
        background-color: rgb(34, 34, 255);
        color: #fff;
        font-size: 16px;
        border-radius: 5px;
    }

    button:hover {
        background-color: rgb(77, 77, 248);
        cursor: pointer;
    }
</style>

<body>
    <div class="container">
        <div class="heading" id="heading"></div>
        <input type="text" placeholder=" X" id="ipt-1">
        <p>is what percent of</p>
        <input type="text" placeholder=" Y" id="ipt-2">
        <button onclick="cal();">Calculate</button>
        <input type="text" placeholder=" Z" id="ipt-3">
    </div>
</body>
<script>
    function cal() {
        // document.write(x + " is what percentage of " + y + " Calculator");

        let x = document.getElementById("ipt-1").value;
        let y = document.getElementById("ipt-2").value;
        let cal = ((x / y) * 100)
        let z = document.getElementById("ipt-3").value = cal;
        // console.log(x + " is what percentage of " + y + " Calculator");
        document.getElementById("heading").innerHTML = (x + " is what percentage of " + y + " Calculator");
    }
</script>

</html>
