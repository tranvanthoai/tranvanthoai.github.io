<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Đăng ký / đang nhập</title>
    <style>
        .wrap {
            width: 800px;
            max-width: 100%;
            height: 500px;
            margin: 18px auto 0;
            display: flex;
            animation: FakeIn 0.4s linear;
        }
        @keyframes FakeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }
        .wrap-1 {
            width: 50%;
        }
        .wrap-1 img {
            width: 100%;
            height: 100%;
        }
        .wrap-2,.wrap-3 {
            width: 50%;
            background-color: rgb(53, 49, 49);
            height: 500px;
        }
        .wrap-2 {
            z-index: 1;
        }
        .wrap-3 {
            display: none;
        }
        .heading {
            margin-left: 60px;
            margin-top: 100px;
            user-select: none;
            
        }
        .heading .heading_1 {
            color: rgba(255, 255, 255,0.15);
            user-select: none;
            animation: mau 0.5s linear infinite;
        }
        @keyframes mau {
            from {
                color: yellow;
            }
            to {
                color: red;
            }
        }
        .heading .heading_2 {
            margin: 0 10px;
            color: rgba(255, 255, 255,0.15);
        }
        .heading .heading_3 {
            color: black;
            padding:8px 10px 6px 10px;
            user-select: none;
            border-bottom: 1px solid green;
            background-color: aqua;
            border-radius: 40%;
        }
        .wrap-2__info {
            margin:30px 0 0 60px;
            width: 200px;
            min-height: 100px;
        }
        .wrap-2__info-name {
            margin-top: 20px;
        }
        .wrap-2__info-name span {
            color: white;
            font-size: 12px;
        }
        .wrap-2__info-name input {
            outline: none;
            margin-top:10px;
            background-color: transparent;
            border: none;
            border-bottom: 1px solid #999;
            color: white;
        }
        .wrap-2__info-pass {
            margin-top: 20px;
        }
        .wrap-2__info-pass span {
            color: white;
            font-size: 12px;
        }
        .wrap-2__info-pass input {
            outline: none;
            margin-top:10px;
            background-color: transparent;
            border: none;
            border-bottom: 1px solid #999;
            color: white;
        }
        .wrap-2__info-email {
            margin-top: 20px;
        }
        .wrap-2__info-email span {
            color: white;
            font-size: 12px;
        }
        .wrap-2__info-email input {
            outline: none;
            margin-top:10px;
            background-color: transparent;
            border: none;
            border-bottom: 1px solid #999;
            color: white;
        }
        .wrap-2__dieukhoan {
            margin:20px 0 0 0;
        }
        .wrap-2__dieukhoan span.span1 {
            color: rgba(255, 255, 255,0.4);
        }
        .wrap-2__dieukhoan span.span2 {
            color: rgba(255, 255, 255,1);
            border-bottom: 1px solid green;
        }
        .submit-btn {
            margin-top: 20px;
        }
        .submit-btn input {
            background-color: aquamarine;
            border: none;
            border-radius: 20px;
            padding:6px 26px 6px;
            color: white;
        }
        .submit-btn span {
            font-size: 12px;
            color: rgba(255, 255, 255,0.4);
        }
        #check-sign-in:checked ~ .wrap-2 {
            display: none;
        }
        #check-sign-in:checked ~ .wrap-3 {
            display: block;
        }
        @media (max-width:800px) {
            .wrap-1 {
                display: none;
                width: 0%;
            }
            .wrap-2,.wrap-3 {
            width: 100%;
            }
            .heading {
            margin-left: 40%;
            margin-top: 90px;
             }
             .wrap-2__info {
            margin:30px 0 0 20%;
            width: 200px;
            min-height: 100px;
            }
            .wrap-2__info-name input,
            .wrap-2__info-pass input,
            .wrap-2__info-email input,
            .submit-btn input {
                width: 350px;
            }
            
        }
    </style>
</head>
<body bgcolor="#ce78a6">
    <div class="wrap">
        <div class="wrap-1">
            <img src="./assets/img/anh-dangky.jpg" alt="">
        </div>
        <input type="checkbox" id="check-sign-in" hidden>
        <div class="wrap-2" >
            <div class="heading">
                <label for="check-sign-in" class="heading_1" style="cursor: pointer;">Sign In</label>
                <span class="heading_2">or</span>
                <span class="heading_3">Sign Up</span>
            </div>
            <form class="wrap-2__info">
                <div class="wrap-2__info-name">
                    <span>FULL NAME</span>
                    <input type="text" name="" id="" placeholder="Enter your full name" required>
                </div>
                <div class="wrap-2__info-pass">
                    <span>PASSWORD</span>
                    <input type="text" name="" id="" placeholder="**************" required>
                </div>
                <div class="wrap-2__info-email">
                    <span>E-MAIL</span>
                    <input type="text" name="" id="" placeholder="Your e-mail goes here" required>
                </div>
                <div class="wrap-2__dieukhoan">
                    <input type="checkbox" name="" id="" required>
                    <span class="span1">I agree all statements in</span>
                    <span class="span2">terms of service</span>
                </div>
                <div class="submit-btn">
                    <input type="submit" value="Sing Up" href="google.com">
                    <span>I'm already member</span>
                </div>
            </form>
        </div>
       
        <div class="wrap-3">
            <div class="heading">
                <span class="heading_3">Sign In</span>
                <span class="heading_2">or</span>
                <label for="check-sign-in" style="cursor: pointer;" class="heading_1">Sign Up</label>
            </div>
            <form class="wrap-2__info">
                <div class="wrap-2__info-name">
                    <span>User Name</span>
                    <input type="text" name="" id="" placeholder="Enter your user name" required>
                </div>
                <div class="wrap-2__info-pass">
                    <span>PASSWORD</span>
                    <input type="text" name="" id="" placeholder="************" required>
                </div>
                <div class="wrap-2__dieukhoan">
                    <input type="checkbox" name="" id="" required>
                    <span class="span1">I agree all statements in</span>
                    <span class="span2">terms of service</span>
                </div>
                <div class="submit-btn">
                    <input type="submit" value="Sing In" href="google.com">
                    
                </div>
            </form>
        </div>

    </div>
</body>
</html>
