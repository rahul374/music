<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Play music </title>
    <style>
        .box{
    width: 90%;
    height: 700px;
    margin: auto;
    /* border: 2px solid red; */
    display: grid;
    grid-template-columns: 33% 33% 33%
    

}
body{
    /* background-image: linear-gradient(rgb(63, 202, 25),rgb(56, 220, 56)); */
    font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
}

h1{
    text-align: center;
    color: cyan;
}
h3{
    font-size: 20px;
    text-align: center;
    color: blue;
}

.a{
    background-image: url('m1.jpg');
   background-repeat: no-repeat; 
   background-size: 100% 100%; 
   margin: 5px 7px;
   border-radius: 20px;
}
.b{
    background-image: url('m2.jpg');
   background-repeat: no-repeat; 
   background-size: 100% 100%; 
   margin: 5px 7px;
   border-radius: 20px;
}
.c{
    background-image: url('m3.jpg');
   background-repeat: no-repeat; 
   background-size: 100% 100%; 
   margin: 5px 7px;
   border-radius: 20px;
}
.d{
    background-image: url('m4.jpg');
   background-repeat: no-repeat; 
   background-size: 100% 100%; 
   margin: 5px 7px;
   border-radius: 20px;
}
.e{
    background-image: url('m5.jpg');
   background-repeat: no-repeat; 
   background-size: 100% 100%; 
   margin: 5px 7px;
   border-radius: 20px;
}
.f{
    background-image: url('m6.jpg');
   background-repeat: no-repeat; 
   background-size: 100% 100%; 
   margin: 5px 7px;
   border-radius: 20px;
}
.g{
    background-image: url('m7.jpg');
   background-repeat: no-repeat; 
   background-size: 100% 100%; 
   margin: 5px 7px;
   border-radius: 20px;
}
.h{
    background-image: url('m8.jpg');
   background-repeat: no-repeat; 
   background-size: 100% 100%; 
   margin: 5px 7px;
   border-radius: 20px;
}
.i{
    background-image: url('m9.jpg');
   background-repeat: no-repeat; 
   background-size: 100% 100%; 
   margin: 5px 7px;
   border-radius: 20px;
}

@media screen and (min-width:200px)and (max-width:480px){
.box{

    height: 600px;
    display: grid;
    grid-template-columns: 50% 50% ;
    /* text-align: center; */

}


.song{
    margin: 10px 20px;
    background-size: 100% 100%;
}




}
@media screen and (min-width:481px)and (max-width:900px){
    .box{
    
        height: 1000px;
        display: grid;
        grid-template-columns: 50% 50% ;
    
    
    }
    .song{
        margin: 10px 20px;
        background-size: 100% 100%;
    }
    .song:hover{
        cursor: pointer;
        border: 5px solid yellow;
    }

    
    
    }
    .song:hover{
        cursor: pointer;
        border: 5px solid yellow;
    }



    </style>
</head>
<body>
    
    <div class="container">
    <h1>MY MUSIC  PLAYER</h1>
    <h3>click on picture for start music</h3>
    <h3>Double click for close music</h3>
    
        <div class="box">
            <div class="a song">a</div>
            <div class="b song ">b</div>
            <div class="c song">c</div>
            <div class="d song">d</div>
            <div class="e song">e</div>
            <div class="f song">f</div>
            <div class="g song">g</div>
            <div class="h song">h</div>
            <div class="i song">i</div>
        </div>
    </div>

    
</body>
<script>
console.log("this is  music tutorial");
let divlenght = document.querySelectorAll('.song').length;
console.log(divlenght);
for (var i = 0; i <= divlenght; ++i) {


    let demo = document.querySelectorAll('.song')[i];
    demo.addEventListener('click', playsong);
     demo = document.querySelectorAll('.song')[i];
    demo.addEventListener('dblclick', pausesong);


    let song1 = new Audio();
    song1.src = "music1.mp3";

    let song2 = new Audio();
    song2.src = "music2.mp3";

    let song3 = new Audio();
    song3.src = "music3.mp3";

    let song4 = new Audio();
    song4.src = "music4.mp3";

    function playsong() {
        var songid = this.innerHTML;
        console.log(songid);

        switch (songid) {
            case "a":
                song4.play();
                break;
            case "b":
                song1.play();
                break;
            case "c":
                song3.play();
                break;
            case "d":
                song4.play();
                break;
            case "e":
                song1.play();
                break;
            case "f":
                song2.play();
                break;
            case "g":
                song3.play();
                break;
            case "h":
                song2.play();
                break;
            case "i":
                song4.play();
                break;
            default:
                console.log('wrong selection');
                break;
        }


    }
    function pausesong() {
        var songid = this.innerHTML;
        console.log(songid);

        switch (songid) {
            case "a":
                song4.pause();
                break;
            case "b":
                song1.pause();
                break;
            case "c":
                song3.pause();
                break;
            case "d":
                song4.pause();
                break;
            case "e":
                song1.pause();
                break;
            case "f":
                song2.pause();
                break;
            case "g":
                song3.pause();
                break;
            case "h":
                song2.pause();
                break;
            case "i":
                song4.pause();
                break;
            default:
                console.log('wrong selection');
                break;
        }


    }
}
</script>
</html>
