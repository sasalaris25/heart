{

    margin: 0;
    padding: 0;
    box-sizing: border-box;

}

body{
    width: 100%;
    height: 100vh;

    display: flex;
    justify-content: center;
    align-items: center;

    background-color: black;
}

.heart{
    width: 100px;
    height: 160px;

    position: relative;

    background-color: red;

    transform-origin: right bottom;

    border-radius: 15px;

    /*transition: .5s ease;*/
    animation: heart 3s ease infinite alternate;


}

@keyframes heart{
    0%{
    transform: rotate(0deg);
    }
    50%{
    transform: rotate(45deg);
    border-top-left-radius: 50px;
    border-top-right-radius: 50px;
    }
    55%{
        transform: rotate(45deg) scale(1);
    }
    60%{
        transform: rotate(45deg) scale(1.2);
    }
    65%{
        transform: rotate(45deg) scale(1);
    }
    70%{
        transform: rotate(45deg) scale(1.2);
    }
    75%{
        transform: rotate(45deg) scale(1);
    }
    80%{
        transform: rotate(45deg) scale(1.2);
    }
    85%{
        transform: rotate(45deg) scale(1);
    }
    90%{
        transform: rotate(45deg) scale(1.2);
    }
    95%{
        transform: rotate(45deg) scale(1);
    }
    100%{
        transform: rotate(45deg) scale(1.2);
        border-top-left-radius: 50px;
        border-top-right-radius: 50px;
    }
}


/*.heart:hover{
    transform: rotate(45deg);
    transition: .5s ease;

    border-top-left-radius: 50px;
    border-top-right-radius: 50px;

}*/

.heart:after{
    content: '';

    width: 100%;
    height: 100%;

    border-radius: 15px;

    transform-origin: left bottom;

    background-color: rgb(192, 0, 0);

    position: absolute;
    /*transition: .5s ease;*/
    animation: heart_after 3s ease infinite alternate;

}

@keyframes heart_after{
    0%{
        transform: rotate(0deg);
        }
        50%{
        transform: rotate(-90deg) translateY(100px);
        border-top-left-radius: 50px;
        border-top-right-radius: 50px;
        }
        100%{
        transform: rotate(-90deg) translateY(100px);
        border-top-left-radius: 50px;
        border-top-right-radius: 50px;
        }
}


/*.heart:hover:after{
    transform: rotate(-90deg) translateY(100px);
    transition: .5s ease;

    border-top-left-radius: 50px;
    border-top-right-radius: 50px;
}*/

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Te amo tanto que não cabe no meu...</title>
    <link rel="stylesheet" href="heart2.css">
</head>
<body>
    <div class="heart"></div>
</body>
</html>
