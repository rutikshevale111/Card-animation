# Card-animation
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>card</title>
    <link rel="stylesheet" href="card.css">
    

</head>
<body>
        <div class="container">
            <div  class="card">
                <div class="imgBx">
                    <img src="/images/plant.jpg" alt="">

                </div>
                <div class="content">
                    <span class="price">
                        <a href="">Forest</a>
                    </span>
                    <ul>
                        <li><b>Plant</b></li>
                        <li>Goa, India</li>
                        <P>Lorem ipsum dolor sit amet consectetur adipisicing elit.</P>
                    </ul>
                </div>
            </div>
            <div class="card">
                <div class="imgBx">
                    <img src="/images/mashroom.jpg" alt="">

                </div>
                <div class="content">
                    <span class="price">
                        <a href="">Forest</a>
                    </span>
                    <ul>
                        <li><b>Mushroom</b></li>
                        <li>Kolkata, India</li>
                        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                    </ul>
                </div>
            </div>
            <div class="card">
                <div class="imgBx">
                    <img src="/images/forest.jpg" alt="">

                </div>
                <div class="content">
                    <span class="price">
                        <a href="">Forest</a>
                    </span>
                    <ul>
                        <li><b>Bridge</b></li>
                        <li>Pune, India</li>
                        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                    </ul>
                </div>
            </div>
        </div>
    </body>
</body>
</html>
</body>
</html>

<!---css file---!>
@import url('https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@400;500;600;700&display=swap');
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Roboto Mono', monospace;
}


.container{
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    height: 100vh;
    background: #a3b18a;
}

.card{
    position: relative;
    width: 320px;
    height: 400px;
    display: flex;
    justify-content: space-between;
    flex-direction: column;
}


.card .imgBx{
    position: relative;
    width: 100%;
    height: 240px;
    border-radius: 15px;
}

.card .imgBx img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 15px;
}

.card .imgBx::before{
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    width: 20px;
    height: 20px;
    background: transparent;
    border-radius: 50%;
    box-shadow: -10px 10px 0 #a3b18a;
}

.card .imgBx::after{
    content: '';
    position: absolute;
    bottom: 68px;
    left: 0;
    width: 20px;
    height: 20px;
    background: transparent;
    border-radius: 50%;
    box-shadow: -10px 10px 0 #a3b18a;
}

.card .content{
    position: relative;
    width: 100%;
    height: 150px;
    background: #344e41;
    border-radius: 15px;
    border-top-left-radius:0 ;
}

.card .content ul{
    padding: 0 20px;
    color: #fff;
    font-size: 18px;
    padding-bottom: 5px;
    list-style: none;
}

.card .content p{
    font-size: 14px;
}

.card .content .price{
    position: absolute;
    top: -52%;
    height: 52%;
    width: 50%;
    background: #344e41;
    border-top: 10px solid #a3b18a;
    border-right: 10px solid #a3b18a;
    border-top-right-radius: 25px;
}

.card .content .price a{
    position: relative;
    background: #fff;
    padding: 10px 20px;
    margin: 15px;
    display: block;
    border-radius: 7px;
    font-weight: 600;
    text-decoration: none;
    text-align: center;
    color: #344e41;
    transition: 0.5s;
    border: 2px solid #344e41;
}

.card .content .price a:hover{
    color: #fff;
    background: #344e41;
    border: 2px solid #fff;
}

.card .content .price::before{
    content: '';
    position: absolute;
    width: 25px;
    height: 25px;
    background: transparent;
    border-radius: 50%;
    box-shadow: -10px -10px 0#a3b18a ;
}

.card .content .price::after{
    content: '';
    position: absolute;
    bottom: 0;
    right: -25px;
    width: 25px;
    height: 25px;
    background: transparent;
    border-radius: 50%;
    box-shadow: -10px 10px 0 #344e41;
}
