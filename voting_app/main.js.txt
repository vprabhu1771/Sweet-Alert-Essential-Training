window.onload = function()
{
    const name = document.getElementById("name");
    
    const age = document.getElementById("age");
    
    const check_btn = document.getElementById("check_process");

    check_btn.addEventListener('click', function(){

        if (age.value >= 18) 
        {
            Swal.fire({
                icon: 'success',
                title: 'Congrats ' + name.value,
                text: 'You are eligible for voting',
            })    
        }
        else
        {
            Swal.fire({
                icon: 'error',
                title: 'Sorry ' + name.value,
                text: 'You are not eligible for voting',
            })
        }

        

    });


}