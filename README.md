/# bemyvalentines.github.io
<html lang="en"><head>
        <link rel="stylesheet" href="./styles.css">
        <title>Will you be my valentine, Esther?</title>
    </head> 
    <body>
        <div class="container">
            <div>
                <h1 class="header_text">Will you be my valentine, Rebecca?</h1>
                <h2 id="please" class="sub_text"></h2>
            </div>
            <div class="gif_container">
                <img id="img" src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExcDdtZ2JiZDR0a3lvMWF4OG8yc3p6Ymdvd3g2d245amdveDhyYmx6eCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/cLS1cfxvGOPVpf9g3y/giphy.gif" alt="Cute animated illustration">
            </div>

            <div class="buttons">
                <button class="btn" id="yesButton" onclick="nextPage()">Yes</button>
                <button class="btn" id="noButton" onmouseover="moveButton()" onclick="moveButton()">No</button>
                <script>
                    function nextPage() {
                        window.location.href = "yes.html";
                    }
                    let i = 0;
                    function moveButton() {
                        var x = Math.random() * (window.innerWidth - document.getElementById('noButton').offsetWidth) - 95;
                        var y = Math.random() * (window.innerHeight - document.getElementById('noButton').offsetHeight) - 58;
                        document.getElementById('noButton').style.left = `${x}px`;
                        document.getElementById('noButton').style.top = `${y}px`;
                        let image = [
                            'https://media0.giphy.com/media/eHWUyxudOQGCulzFFR/giphy.gif',
                            'https://media0.giphy.com/media/hm8GqsZ2RteDRWW7OS/giphy.gif',
                            'https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExbnA5ZnV2ZHV6enQ4cTl1bXdyY2g5OGQ5Z2s0YnpxeWxzampjOHQ4dyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/lPM06f2zvk94jBAzlP/giphy.gif',
                            'https://media.tenor.com/mDHFdvLgRaIAAAAi/so-sad-sad-face.gif',
                            'https://media.tenor.com/3VM2_MnIbNgAAAAi/crying-sobbing.gif',
                        ]

                        let text = [
                            'Please, say yes!',
                            'I am begging you',
                            'I am not giving up!',
                            'Please.....',
                            'Please..........'
                            ]
                        document.getElementById('please').innerHTML = text[i];

                        document.getElementById('img').src =  image[i];
                        i = i < image.length - 1 ? i + 1 : 0;
                    }
                </script> 
            </div>
        </div>
       
     
</body></html>
