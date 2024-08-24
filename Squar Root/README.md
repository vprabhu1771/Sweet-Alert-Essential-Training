# Squar Root
 
1. open `index.html`

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>

    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>

    <script src="main.js"></script>
</head>
<body>

    <input type="text" id="sqrt" placeholder="Enter any integer">

    <input type="button" value="check" id="check_process">
    
</body>
</html>
```

2. open `main.js`

```
window.onload = function()
{
       
    const sqrt = document.getElementById("sqrt");
    
    const check_btn = document.getElementById("check_process");

    check_btn.addEventListener('click', function(){

        Swal.fire({
            text: parseInt(sqrt.value) * parseInt(sqrt.value),
        })    

    });

}
```

![Image](3.PNG)

![Image](4.PNG)