<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   @import url(<link rel="preconnect" href="https://fonts.googleapis.com">
   <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
   <link href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">)
    <link rel="stylesheet" href="cat.css">
    <title>Document</title>
</head>
<body>

    

    <header>
        <a href="#" class="logo">catarina</a>
        <nav>
            <a href="#" class="active">home</a>
            <a href="#">serviços</a>
            <a href="#">contato</a>
        </nav>
    </header>
    <section class="home">
        <div class="home-img">
            <img src="cati.jpeg" alt="">
        </div>
        <div class="home content">
            <h1>Oie! Eu sou a  <span>catarina</span></h1>
            
            <p>Oie! Eu sou a Catarina tenho 16 anos e atualmente trabalho no ramo de digital influencer e marketing! Quero expandir, faço vídeos da sua loja, provador de roupa e calçados. Faço vídeo mostrando seu negócio, vídeos com edição e flayers.</p>
            <div class="social-icons">
                <a href=""> <i class="fa-brands fa-instagram"></i></a>
            </div>
        </div>
    </section>
</body>
</html>









*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    font-size: 'poppins',sans-serif;

}

html{
    font-size: 62.5%;
}

body{
    width: 100%;
    height: 100vh;
    overflow-x: hidden;
    background-color: black;
    color: white;
}

header{
    margin-top: 20px;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 1rem 9%;
    background-color: transparent;
    filter: drop-shadow(10px);
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}

.logo{
    font-size: 3rem;
    color: pink;
    font-weight: 800;
    cursor: pointer;
    transition: 0.5s ease;

}

.logo.hover{
    transform: scale(1.1);
}

nav a{
    font-size: 1.8rem;
    color: white;
    margin-left: 4rem;
     font-weight:500 ;
     transition: 0.3s ease;
     border-bottom: 3px solid transparent;
}

nav a:hover,
nav a.active{
    color: pink;
    border-bottom: 3px solid pink;
}

@media(max-width:995px){
    nav{
        position: absolute;
        display: none;
        top: 0;
        right: 0;
        width: 40%;
        border-left: 3px solid pink;
        border-bottom: 3px solid pink;
        border-bottom-left-radius: 2rem;
        padding: 1rem solid;
        background-color: rgba(16,16,16);
        border-top: 0.1rem solid rgba(0,0,0,0.1);
    }


nav.active{
    display: block;
}

nav a{
    display: block;
    font-size: 2rem;
    margin: 3rem 0;

}

nav a:hover,
nav a.active{
    padding: 1rem;
    border-radius: 0.5rem;
    border-bottom: 0.5rem solid pink;
}

}
section{
    min-height: 100vh;
    padding: 5rem 9% 5rem;

}

.home{
    display: flex;
    justify-content: center;
    align-items: center;
    gap:8rem;
    background-color: rgb(0, 0, 0);
}

.home .home-content h1{
    font-size: 6rem;
    font-weight: 700;
    line-height: 1.3;
    font-size: 200px;
}

span{
    color: pink;
}

.home-content h3{
    font-size: 4rem;
    margin-bottom: 1rem;
    font-weight: 700;

}

.home-content p{
    font-size: 1.6rem;
}

.home-img{
    border-radius: 50%;
}

.home-img img{
    position: relative;
    width:32vw ;
    border-radius: 50%;
    box-shadow: 0 0 25px solid pink;
    cursor: pointer;
    transition: 0.2s linear;

}

.home-img img:hover{
    font-size: 1.8rem;
    font-weight: 500;

}

.socail-icons a {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 4rem;
    height: 4rem;
    background-color: transparent;
    border: 0.2rem solid pink;
    font-size: 2rem;
    border-radius: 50%;
    margin: 3rem 1.5rem 3rem 0;
    transition: 0.3s ease;
    color: white;
}

.social-icons a:hover{
    color: black;
    transform: scale(1.3) translateY(-5px);
    background-color:pink ;
    box-shadow: 0 0 25px pink;
}

.btn{
    display: inline-block;
    padding: 1rem 2.8rem;
    border-radius: 4rem;
    font-size: 1.6rem;
    color: pink;
    letter-spacing: 0.3rem;
    font-weight: 600;
    transition: 0.3 ease;
    cursor: pointer;
}

.btn:hover{
    transform: scale3d(1.03);
    background-color: pink;
    color: black;
    box-shadow: 0 0 25px pink;
}

.typing-text{
    font-size: 34px;
    font-weight: 600;
    min-width: 280px;
}

.typing-text span{
    position: relative;
}

.typing-text span:before{
content:"marketing e conteudo digital";
color: black;
animation: words 20s infinite;
}


.typing-text span:after{
   
    background-color: black;
    position: absolute;
    width: calc(100%+8px);
    height: 100%;
    border-left: 3px solid  black;
    right: -8;
    animation: "cursor" 0.6s infinite;
}

@keyframes cursor{
    to{
        border-left: 3px solid pink;
    }
}

@keyframes words{
    0%,20%{
        content:"marketing digital";
    }

    21%,40%{
        content:"conteudo digital";
    }

    41%,60%{
        content:" influencer"
    }

    61%, 80%{
        content: "tik toker";
    }

    81%,100%{
        content: "focada";
    }
}

@media(max-width:1000px){
    .home{
        gap: 4rem;
    }
}

@media (max-width:995px) {
    .home{
        flex-direction: column;
        margin: 5rem 4rem;
    }

    .home .home-content h3{
        font-size: 2.5rem
    }

    .home-content h1{
        font-size: 5rem;
    }

    .home-img img{
        width: 70vw;
        margin-top: 4rem;
    }
}
