<!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="./styles.css">
        
    </head> 
    <body>
        <div class="container">
            <div >
                <h1 class = "header_text">Do you wanna go out with me, my cochinito?</h1>
                <h1 class = "header_text">Are you free tonight?</h1>
            </div>
            <div class="gif_container">
                <img src="https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExcW50OTRyNzgxd2l0d3g4MDQ1N2h6b3lhaXBkY2R4aHByMXJxbGl5bSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/TRtE00FO5ZGl3qau5D/giphy.gif" alt="Cute animated illustration">
            </div>
            <div class = "buttons">
                <button class="btn" id = "yesButton" onclick="nextPage()">Yes</button>
                <button class="btn" id="noButton" onmouseover="moveButton()" onclick="moveButton()">No</button>
                <script>
                    function nextPage() {
                        window.location.href = "yes.html";
                    }
                    
                    function moveButton() {
                        var x = Math.random() * (window.innerWidth - document.getElementById('noButton').offsetWidth) - 85;
                        var y = Math.random() * (window.innerHeight - document.getElementById('noButton').offsetHeight) - 48;
                        document.getElementById('noButton').style.left = `${x}px`;
                        document.getElementById('noButton').style.top = `${y}px`;
                    }
                </script> 
            </div>
        </div>
       
    </body> 
</html>
