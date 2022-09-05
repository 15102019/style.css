
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Montserrat', sans-serif
}
body{
    width: 100%;
    height: 100%;
    background: url(imagem/fundo-claro-em-rosa-pastel_53876-120097.webp);
    background-size: cover;

}

header{
    width: 100%;
    height: 80px;
    background: rgb(218, 165, 174);
    display: flex;
    align-items: center;
    justify-content: space-around;
    position: fixed;
    z-index: 99;
}
header .logo{
    width: 50%;
}
header .logo img{
    width: 140px;
}
header .menu ul{
    display: flex;
}
header .menu ul li{
    padding: 0 20px;
    list-style: none;
}
header .menu ul li a{
    text-decoration: none;
    text-transform: uppercase;
    color: #fff;
    transition: 0.5s ease;
}
header .menu ul li a:hover{
    color: rgb(206, 116, 131);
}
header .menu-mobile{
    display: none;
}
header .btn-mobile{
    display: none;
}

/*===== Principal Início =====*/

#home .container{
    width: 100%;
    height: 100vh;
    background: url(imagem/Screenshot_20220905-102457_LinkedIn.jpg);
    background-size: cover;
    display: flex;
    justify-content: space-between;  
}
    
#home .container .icons{
    width: 10%;
    height: 80vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 0 60px;
    position: fixed;
    z-index: 999;
}
#home .container .icons ion-icon{
    padding: 30px 0;
    font-size: 2rem;
    color: #fff;
    transition: 0.5s ease;
}
#home .container .icons ion-icon:hover{
    color: rgb(220, 80, 103);
}
#home .container .title{
    width: 100%;
    height: 80vh;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: center;
    padding: 0 60px;
}
#home .container .title h1{
    color: #fff;
    text-transform: uppercase;
    font-size: 8rem;
    letter-spacing: 5px;
}
#home .container .title h2{
    color: #fff;
    text-transform: uppercase;
    letter-spacing: 40px;
    font-size: 3rem;
    margin-left: 30px;
}
#home .container .title h3{
    color: #fff;
    text-transform: uppercase;
    font-size: 1.2rem;
    letter-spacing: 20px;
    margin-top: 30px;
    margin-left: 35px;

}
/*===== sobremim =====*/

#about .container{
    width: 100%;
    height: 100vh;
    background: url(imagem/fundo-claro-em-rosa-pastel_53876-120097.webp);
    background-size: cover;
    display: flex;
    justify-content: space-between;
}
#about .container .title{
    width: 90%;
    height: 100vh;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    padding: 0 60px;
}
#about .container .title h1{
    color: black;
    text-transform: uppercase;
    font-size: 2rem;
    text-align: left;
}
#about .container .title p{
    color: black;
    width: 500px;
    margin-top: 30px;
}


/*===== portfolio =====*/
#port .container{
    width: 100%;
    height: 100vh;
    background: url(imagem/fundo-claro-em-rosa-pastel_53876-120097.webp);
    background-size: cover;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    
}
#port .container input[type=radio]{
    display: none;
}
#port .container .card{
    position: absolute;
    width: 40%;
    height: 80%;
    left: 0;
    right: 0;
    margin: 150px auto;
    display: flex;
    align-items: flex-start;
    justify-content: center;
    box-shadow: 0 0 10px 0 rgb(217, 78, 102);
    transition: 0.4s ease;
    cursor: pointer;
}
#port .container .card img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 10px;
}
#port .container .card h1{
    position: absolute;
    z-index: 9;
    color: rgb(209, 109, 109);
    font-size: 3rem;
    margin-top: 20px;
}
#port .container .card p{
    position: absolute;
    z-index: 9;
    width:400px ;
    color: rgb(238, 85, 111);
    margin-top: 200px;
    text-align: justify;
    font-size: 2rem;
}
#port .container .card button{
    position: absolute;
    z-index: 9;
    margin-top: 400px;
    padding: 10px 20px;
    border-radius: 20px;
    border: none;
    color: black;
    background: rgb(214, 86, 108);
    text-transform: uppercase;
    cursor: pointer;
}
#port .container .cards{
    position: relative;
    width: 100%;
    height: 100%;
}
#item-1:checked ~ .cards #song-3,
#item-2:checked ~ .cards #song-1,
#item-3:checked ~ .cards #song-2{
    transform: translateX(-40%) scale(0.8);
    opacity: 0.4;
    z-index: 0;
}
#item-1:checked ~ .cards #song-2,
#item-2:checked ~ .cards #song-3,
#item-3:checked ~ .cards #song-1{
    transform: translateX(40%) scale(0.8);
    opacity: 0.4;
    z-index: 0;
}
#item-1:checked ~ .cards #song-1,
#item-2:checked ~ .cards #song-2,
#item-3:checked ~ .cards #song-3{
    transform: translateX(0) scale(1);
    opacity: 1;
    z-index: 1;
}

/*===== Contact =====*/
#contact .container{
    width: 100%;
    height: 100vh;
    background: url(imagem/fundo-claro-em-rosa-pastel_53876-120097.webp);
    background-size: cover;
    transition: background 0.4s ease-in;
}
#contact .container .content-contact{
    width: 80%;
    height: 60vh;
    margin: 0 auto;
    padding: 200px 0;
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
}
#contact .content-contact .contact-left{
    width: 50%;
    display: flex;
    flex-direction: column;
    color: black;
}
#contact .content-contact .contact-left h1{
    font-size: 2rem;
    text-transform: uppercase;
}
#contact .content-contact .linha{
    width: 350px;
    height: 3px;
    background: black;
    margin-top: 10px;
    margin-bottom: 10px;
}
#contact .content-contact .contact-left ion-icon{
    font-size: 2rem;
    padding: 20px 0;
}
#contact .content-contact .contact-left span{
    font-size: 1.2rem;
    padding: 5px 0;
}
#contact .content-contact .contact-right{
    width: 50%;
    display: flex;
    flex-direction: column;
    color: black;
}
#contact .content-contact .contact-right h1{
    font-size: 2rem;
    text-transform: uppercase;
}
#contact .content-contact .contact-right input[type=email],
#contact .content-contact .contact-right input[type=text]{
    border-radius: 20px;
    border: none;
    padding: 15px 20px;
    margin-bottom: 20px;
    font-size: 1.2rem;
    font-weight: 600;
    outline: none;
}
#contact .content-contact .contact-right textarea{
    width: 100%;
    height: 120px;
    border-radius: 20px;
    border: none;
    margin-bottom: 20px;
    font-size: 1.2rem;
    font-weight: 600;
    outline: none;
    padding: 15px 20px;
}


/*===== Resposive =====*/

@media screen and (max-width: 1280px){
    #home .container .icons ion-icon{
        font-size: 1.5rem;
    }
    #port .container .card h1{
        font-size: 5rem;
    }
    #port .container .card p{
        width: 280px;
        font-size: 0.8rem;
    }
}
@media screen and (max-width: 960px){
    body{
        background: url(imagem/fundo-claro-em-rosa-pastel_53876-120097.webp);
    }
    header{
        background: none;
    }
    header .logo{
        width: 600px;
    }
    header .menu{
        display: none;
    }
    header .btn-mobile{
        display: block;
    }
    header .btn-mobile ion-icon {
        color: black;
        font-size: 1.5rem;
    }
    header .menu-mobile{
        display: none;
        width: 50%;
        height: 20vh;
        box-shadow: 0 0 15px 0 rgb(213, 80, 102);
        position: fixed;
        top: 20px;
        border-radius: 10px;
        background: rgb(146, 20, 41);
    }
    header .menu-mobile ul{
        text-align: center;
    }
    header .menu-mobile ul li{
        list-style: none;
        padding: 12px 0;
    }
    header .menu-mobile ul li a{
        text-decoration: none;
        text-transform: uppercase;
        color: #fff;
    }
    #home .container .icons{
        padding: 0 20px;
    }
    #home .container .title{
        align-items: center;
    }
    #home .container .title h1{
        font-size: 5rem;
    }
    #home .container .title h2{
        font-size: 1.2rem;
    }
    #home .container .title h3{
        font-size: 0.9rem;
    }
    #about .container .title{
        align-items: center;
    }
    #about .container .box-title{
        width: 100%;
        height: 40vh;
    }
    
    #contact .container .content-contact{
        width: 100%;
        height: 100vh;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }
    #contact .content-contact .contact-left h1{
        font-size: 1.5rem;
    }
    #contact .content-contact .contact-left ion-icon{
        font-size: 1.5rem;
        padding: 5px 0;
    }
    #contact .content-contact .contact-left span{
        font-size: 1rem;
        padding: 5px 0;
    }
    #contact .content-contact .contact-right h1{
        font-size: 1.5rem;
        margin-top: 80px;
    }
    #contact .content-contact .contact-right input[type=email],
    #contact .content-contact .contact-right input[type=text]{
        padding: 10px 15px;
        font-size: 1rem;
    }
    #contact .content-contact .contact-right textarea{
        padding: 10px 15px;
        font-size: 1rem;
    }
}
@media screen and (max-width: 750px){
    header{
        padding: 10px;
    }
    #home .container .title h2{
        letter-spacing: 30px;
    }
    #home .container .title h3{
        letter-spacing: 10px;
    }
    #about .container .title{
        padding: 10px 60px;
    }
    #about .container .title p{
        width: 100%;
        margin-top: 30px;
    }
    #port .container .card{
        width: 60%;
        height: 60%;
    }
}
