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
<script src="music.js"></script>
</html>
