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