<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dukaan</title>
    <!-- <script src="https://kit.fontawesome.com/a076d05399.js"></script> we write js above the page so some time our html block the content of js which is written first then html so write below -->
    <link href="https://fonts.googleapis.com/css2?family=PT+Serif:ital@1&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0px;
            padding: 0px;
            box-sizing: border-box;
        }

        /* body {
            /* background-image: linear-gradient(rgba(177, 220, 255, 0.05), white); 
        } */

        header {
            position: absolute;
            top: 0px;
            left: 0px;
            /* background-image: url('shop2.jpg'); */
            /* background-image: linear-gradient(#32d9d8 , #ffbee2); */
            /* background-image: linear-gradient(#32d9d8, #ffbee2); */
            /* background-repeat: no-repeat;
            background-size: cover;
            background-position: center; */
            background-color: rgb(0, 0, 73);
            ;
            border-radius: 1px;
            width: 100%;
            height: 40px;
            z-index: -1;
            display: flex;
            justify-content: center;
            align-items: center;
            position: sticky;
            top: 0px;
            z-index: 1;
            /* opacity: 0.8; */
        }

        .company-name {
            color: white;
            margin-left: 10px;
        }

        .company-name:hover {
            cursor: pointer;
        }

        .container {
            height: 40px;
            display: flex;
            justify-content: center;
            /* margin:0px 20px; */
            color: black;
            background-color: #8194e4;
        }

        #search1 {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 1100px;
            /* margin-right:105.34px; */

        }


        .login {
            background-color: #8194e4;
            border-radius: 8px;
            padding: 10px;
            color: white;
            margin: 3px;

        }

        .signUp {
            background-color: #8194e4;
            border-radius: 10px;
            padding: 10px;
            color: white;
            margin-right: 5px;
        }

        button:hover {
            background-color: #6b7ece;
            color: darkblue;
            cursor: pointer;
        }

        .search {
            /* width:100px;  */
            display: flex;
            height: 40px;
            /* cursor: pointer; */
            /* padding : 15px 10px;  */
            align-items: center;
            justify-content: center;
            border-radius: 30px;
            /* box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.4); */
            cursor: pointer;
            /* border: 2px solid black; */
        }

        .search input {
            width: 0px;
            /* border-radius: 20px; */
            /* padding : 5px 20px; */
            border: none;
            outline: none;
            transition: 0.7s;
            transition-timing-function: ease-in-out;
            font-weight: 900;
            background: transparent;

        }

        #search {
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            /* background-image: linear-gradient(aliceblue, rgba(170, 249, 224, 0.3)); */
            background-color: white;
            z-index: -1;
            height: 30px;
            width: 30px;
            box-shadow: 4px 4px 5px rgba(0, 0, 0, 0.8);
            border-radius: 15px;
            /* cursor: pointer; */
        }

        .search a .fa {
            color: black;
            font-size: 20px;

        }

        .search:hover input {
            /*as input don't have widht = 0 so this line state that when you touch search so hover will apply on input . now we don't do input:hover bcz width of input is 0 so how we touch*/
            width: 400px;
            /* background-image: linear-gradient(white ,rgb(120, 255, 172)); */
            background-color: white;
            color: black;
            padding: 5px 20px;
            border-bottom: 3px solid black;
            border-radius: 30px;
        }


        .h1 {
            margin-top: 0px;

            /* border: 2px solid black; */
            /* background-color: antiquewhite; s*/
        }

        .boxes {
            display: flex;
            justify-content: space-between;
        }

        .box {
            margin: 10px 10px;
            height: 300px;
            width: 200px;
            border-radius: 10px;
            /* border : 2px solid black; */
        }

        #box-1 {
            background-image: url('girl.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
        }

        #box-2 {
            background-image: url('makeup.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
        }

        #box-3 {
            background-image: url('shop3.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
        }

        #box-4 {
            background-image: url('men.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
        }

        .b1 {
            margin: 20px 0px;
            text-align: center;
        }

        .items {
            margin: 0px 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            list-style: none;
        }

        .items1 {
            font-family: cursive;
            color: white;
            font-weight: bold;
            font-size: 16px;
            padding: 5px 0px;
            text-decoration: none;
            transition: transform;
            transition-duration: 275ms;
            transition-timing-function: ease;
        }

        .items1:hover {
            cursor: pointer;
            text-decoration: underline;
            text-decoration-color: rgb(147 51 234);
            transform: scale(1.2);
            /* font-size: 23px; */
            /* font-stretch: expanded; */
            color: blue;
        }

        .style1 {
            transition: background-image;
            transition-duration: 0.3s;
            text-decoration: none;
            font-size: 20px;
            font-family: cursive;
            transition-timing-function: ease;
            color: black;
        }

        .style1:hover {
            box-shadow: 8px 8px 8px 2px gray;
            border-radius: 20px;
            padding: 0px 5px;
            background-image: linear-gradient(rgb(253, 253, 253), rgb(27, 237, 108));
        }

        .banner {
            background-image: url('banner3.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            margin: 20px 0px;
            height: 200px;
            transition: all;
            transition-duration: 1.3s;
            transition-timing-function: ease;
            border-radius: 10px;
        }

        .banner:hover {
            cursor: pointer;
            transform: scale3d(0.8, 0.8, 0.8);
            border-radius: 200px;
            /* background-size: contain; */
        }

        .sports {
            display: flex;
            justify-content: center;
            /* border: 2px solid black; */
            height: 300px;
            margin: 5px;
            /* background-color: aliceblue; */
        }

        .sport {

            /* border: 2px solid black; */
            margin: auto;
        }

        #sport-1 {
            margin: auto;
            background-image: url('cricket.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;
        }

        #sport-2 {
            margin: auto;
            background-image: url('football1.webp');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;

        }

        #sport-3 {
            margin: auto;
            background-image: url('golf.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;

        }

        #sport-4 {
            margin: auto;
            background-image: url('badminton.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;
        }

        .sp {
            margin: 20px 0px;
            text-align: center;
            transition: all;
            transition-duration: 0.4s;
            transition-timing-function: ease;
        }

        .sp:hover {
            cursor: pointer;
            transform: translateX(18px);
            color: white;
            background-color: black;
            padding: 5px 0px;
            border-radius: 40px;
        }

        #heading-1 {
            background-image: url('sport.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            transition: all;
            transition-duration: 1.3s;
            transition-timing-function: ease;
            width: 300px;

        }

        #heading-1:hover {
            cursor: pointer;
            /*border-bottom: 2px solid purple;This hover property is used by code with harry but not in image . he used it in text*/
            transform: rotate3d(1, 1, 1, 45deg);

        }

        /* This is for electronics part*/
        .electronics {
            display: flex;
            justify-content: center;
            /* border: 2px solid black; */
            height: 300px;
            margin: 5px;
            /* background-color: aliceblue; */
        }

        .electronic {

            /* border: 2px solid black; */
            margin: auto;
        }

        #electronic-1 {
            margin: auto;
            background-image: url('iphone.jpg');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;
        }

        #electronic-2 {
            margin: auto;
            background-image: url('macbook.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;

        }

        #electronic-3 {
            margin: auto;
            background-image: url('tv.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;

        }

        #electronic-4 {
            margin: auto;
            background-image: url('camera.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;
        }

        .ece {
            margin: 20px 0px;
            text-align: center;
            transition: all;
            transition-duration: 0.4s;
            transition-timing-function: ease;
        }

        .ece:hover {
            cursor: pointer;
            transform: translateX(18px);
            color: white;
            background-color: black;
            padding: 5px 0px;
            border-radius: 40px;
        }

        #heading-2 {
            background-image: url('electronic.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            transition: all;
            transition-duration: 1.3s;
            transition-timing-function: ease;
            width: 300px;

        }

        #heading-2:hover {
            cursor: pointer;
            /*border-bottom: 2px solid purple;This hover property is used by code with harry but not in image . he used it in text*/
            transform: rotate3d(1, 1, 1, 45deg);

        }

        /* This is for fashion part*/
        .fashions {
            display: flex;
            justify-content: center;
            /* border: 2px solid black; */
            height: 300px;
            margin: 5px;
            /* background-color: aliceblue; */
        }

        .fashion {

            /* border: 2px solid black; */
            margin: auto;
        }

        #fashion-1 {
            margin: auto;
            background-image: url('shirts.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;
        }

        #fashion-2 {
            margin: auto;
            background-image: url('tops.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;

        }

        #fashion-3 {
            margin: auto;
            background-image: url('watches.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;

        }

        #fashion-4 {
            margin: auto;
            background-image: url('shoes.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;
        }

        .fsn {
            margin: 20px 0px;
            text-align: center;
            transition: all;
            transition-duration: 0.4s;
            transition-timing-function: ease;
        }

        .fsn:hover {
            cursor: pointer;
            transform: translateX(18px);
            color: white;
            background-color: black;
            padding: 5px 0px;
            border-radius: 40px;
        }

        #heading-3 {
            background-image: url('fashion.webp');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
            transition: all;
            transition-duration: 1.3s;
            transition-timing-function: ease;
            width: 300px;

        }


        #heading-3:hover {
            cursor: pointer;
            /*border-bottom: 2px solid purple;This hover property is used by code with harry but not in image . he used it in text*/
            transform: rotate3d(1, 1, 1, 45deg);
        }

        /* This is for Home part*/
        .homes {
            display: flex;
            justify-content: center;
            /* border: 2px solid black; */
            height: 300px;
            margin: 5px;
            /* background-color: aliceblue; */
        }

        .home {

            /* border: 2px solid black; */
            margin: auto;
        }

        #home-1 {
            margin: auto;
            background-image: url('fridge.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;
        }

        #home-2 {
            margin: auto;
            background-image: url('ac.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;

        }

        #home-3 {
            margin: auto;
            background-image: url('paint.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;

        }

        #home-4 {
            margin: auto;
            background-image: url('beds.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            /* border: 2px solid black; */
            height: 200px;
            width: 200px;
        }

        .hms {
            margin: 20px 0px;
            text-align: center;
            transition: all;
            transition-duration: 0.4s;
            transition-timing-function: ease;
        }

        .hms:hover {
            cursor: pointer;
            transform: translateX(18px);
            color: white;
            background-color: black;
            padding: 5px 0px;
            border-radius: 40px;
        }

        #heading-4 {
            background-image: url('homes.webp');
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            width: 300px;
            transition: all;
            transition-duration: 1.3s;
            transition-timing-function: ease;

        }

        #heading-4:hover {
            cursor: pointer;
            /*border-bottom: 2px solid purple;This hover property is used by code with harry but not in image . he used it in text*/
            /* transform: rotate3d(1, 1, 1, 45deg); */
            transform: rotate3d(1, 1, 1, 45deg);

        }

        .footer-1 {
            display: flex;
            height: 300px;
            /* border: 2px solid black; */
            justify-content: space-between;
            background-color: rgb(0, 0, 26);
            color: aliceblue;

        }

        .foot {
            display: flex;
            flex-direction: column;
            justify-content: center;
            /* border: 2px solid black; */
            width: 303px;
        }

        .about {
            text-align: center;
            margin: 3px 0px;
        }

        .about:hover {
            cursor: pointer;
            color: aquamarine;
            text-decoration-line: underline;
        }

        .help {
            text-align: center;
            margin: 3px 0px;
        }

        .help:hover {
            cursor: pointer;
            color: aquamarine;
            text-decoration-line: underline;
        }

        .policy {
            text-align: center;
            margin: 3px 0px;
        }

        .policy:hover {
            cursor: pointer;
            color: aquamarine;
            text-decoration-line: underline;
        }

        .social {
            text-align: center;
            margin: 3px 0px;
        }

        .social:hover {
            cursor: pointer;
            color: aquamarine;
            text-decoration-line: underline;
        }

        #ft {
            text-align: center;
            font-family: 'PT Serif', serif;
            margin-bottom: 10px;
            color: #7185dc;
        }

        #foo {
            margin-top: 47px;
        }

        hr {

            height: 0.1px;

        }

        .footer-2 {
            display: flex;
            height: 50px;
            width: 100%;
            background-color: rgb(0, 0, 26);
            color: aliceblue;
            justify-content: space-evenly;

        }

        .foot-1 {
            margin-top: 15px;
            color: white;
        }

        .foot-1:hover {
            cursor: pointer;
            color: #7185dc;
            text-decoration-line: underline;
        }

        .img {
            margin: 13px -30px;
        }

        .icon {
            margin-top: 10px;
            height: 30px;
            width: 40px;
        }

        .icons {
            display: flex;
        }

        .hover1 {
            transition: all;
            transition-duration: 0.3s;
            transition-timing-function: ease-in;
        }

        .hover1:hover {
            cursor: pointer;
            /* opacity:0.9; THis will create problem as image is translucent (that is, content behind the element can be seen) . so back content is also visible along with this*/
            transform: scale(1.1);
            box-shadow: 10px 10px 8px 2px gray;
            /* opacity:0.8; */
            border-radius: 30px;



        }
    </style>
</head>

<body>
    <header>
        <h2 class="company-name">Megashop</h2>
        <div id="search1">
            <div class="search">
                <input type="text" placeholder="search items">
                <a href="#" id="search">
                    <i class="fa fa-search" aria-hidden="true"></i>
                </a>
            </div>
        </div>

        <button class="login">Login</button>
        <button class="signUp">SignUp</button>

    </header>
    <nav class="navbar">
        <ul class="container">
            <li class="items"> <a href="" class="items1 items-1">Home</a> </li>
            <li class="items"> <a href="" class="items1 items-2">Electronics</a> </li>
            <li class="items"> <a href="" class="items1 items-3">Fashion</a> </li>
            <li class="items"> <a href="" class="items1 items-4">Grocery</a> </li>
            <li class="items"> <a href="" class="items1 items-5">Top Deals</a> </li>
            <li class="items"> <a href="" class="items1 items-6"> Customer Services</a></li>
        </ul>
    </nav>

    <div class="h1">
        <div class="boxes">
            <div class="boxes-1">
                <div class="b1"><a href="" class="style1">Styles for women</a></div>
                <div class="box hover1" id="box-1"></div>
            </div>
            <div class="boxes-2">
                <div class="b1"><a href="" class="style1">Explore Fashion</a> </div>
                <div class="box hover1" id="box-2"></div>
            </div>
            <div class="boxes-3">
                <div class="b1"><a href="" class="style1"> All in one</a></div>
                <div class="box hover1" id="box-3"></div>
            </div>
            <div class="boxes-4">
                <div class="b1"><a href="" class="style1">Men's Style</a> </div>
                <div class="box hover1" id="box-4"></div>
            </div>

        </div>
    </div>
    <!--This is for sale banner thing-->

    <div class="banner"></div>
    <!--This is for electronics thing-->

    <div class="sports">
        <div id="heading-1"></div>
        <div class="sport">
            <div id="sport-1" class="hover1"></div>
            <h3 class="sp"> Cricket</h3>
        </div>

        <div class="sport">
            <div id="sport-2" class="hover1"></div>
            <h3 class="sp"> Football</h3>
        </div>
        <div class="sport">
            <div id="sport-3" class="hover1"></div>
            <h3 class="sp"> Golf</h3>
        </div>
        <div class="sport">
            <div id="sport-4" class="hover1"></div>
            <h3 class="sp"> Badminton</h3>
        </div>
    </div>

    <!--This is for electronics thing-->
    <div class="electronics">
        <div id="heading-2"></div>
        <div class="electronic">
            <div id="electronic-1" class="hover1"></div>
            <h3 class="ece">Mobiles</h3>
        </div>

        <div class="electronic">
            <div id="electronic-2" class="hover1"></div>
            <h3 class="ece">Laptops</h3>
        </div>
        <div class="electronic">
            <div id="electronic-3" class="hover1"></div>
            <h3 class="ece">Televisions</h3>
        </div>
        <div class="electronic">
            <div id="electronic-4" class="hover1"></div>
            <h3 class="ece">Cameras</h3>
        </div>
    </div>
    <!--This is Fashion corner-->
    <div class="fashions">
        <div id="heading-3"></div>
        <div class="fashion">
            <div id="fashion-1" class="hover1"></div>
            <h3 class="fsn">Shirts & Pants</h3>
        </div>

        <div class="fashion">
            <div id="fashion-2" class="hover1"></div>
            <h3 class="fsn">Tops & Dresses</h3>
        </div>
        <div class="fashion">
            <div id="fashion-3" class="hover1"></div>
            <h3 class="fsn">Watches</h3>
        </div>
        <div class="fashion">
            <div id="fashion-4" class="hover1"></div>
            <h3 class="fsn">Shoes</h3>
        </div>
    </div>
    <!--This is Home  corner-->
    <div class="homes">
        <div id="heading-4"></div>
        <div class="home">
            <div id="home-1" class="hover1"></div>
            <h3 class="hms">Fridges</h3>
        </div>

        <div class="home">
            <div id="home-2" class="hover1"></div>
            <h3 class="hms">Air Conditioners</h3>
        </div>
        <div class="home">
            <div id="home-3" class="hover1"></div>
            <h3 class="hms">Paints</h3>
        </div>
        <div class="home">
            <div id="home-4" class="hover1"></div>
            <h3 class="hms">Beds</h3>
        </div>
    </div>
    <footer class="footer-1">
        <div class="foot" id="foo">
            <div id="ft">ABOUT</div>
            <div class="about">Contact Us</div>
            <div class="about">About Us</div>
            <div class="about"> Careers</div>
            <div class="about"> Megashop Stories</div>
            <div class="about">Press</div>
            <div class="about">Corporate Information</div>
        </div>
        <div class="foot">
            <div id="ft"> HELP</div>
            <div class="help"> Payments</div>
            <div class="help"> Shipping</div>
            <div class="help"> Cancellation & Returns</div>
            <div class="help"> Report Infringement</div>
        </div>
        <div class="foot">
            <div id="ft">POLICY</div>
            <div class="policy">Return Policy</div>
            <div class="policy"> Terms Of Use</div>
            <div class="policy">Security</div>
            <div class="policy"> Privacy</div>
        </div>
        <div class="foot">
            <div id="ft">SOCIAL</div>
            <div class="social">Facebook</div>
            <div class="social">Instagram</div>
            <div class="social"> YouTube</div>
            <div class="social">Twitter</div>
        </div>
    </footer>
    <hr>
    <footer class="footer-2">
        <div class="icons"><img src="seller.png" alt="" class="icon">
            <div class="foot-1">Become a Seller</div>
        </div>
        <div class="icons">
            <img src="advertise.png" alt="" class="icon">
            <div class="foot-1">Advertise</div>
        </div>
        <div class="icons">
            <img src="gift.png" alt="" class="icon">
            <div class="foot-1">Gift Cards</div>
        </div>
        <div class="icons">
            <img src="helpcenter.png" alt="" class="icon">
            <div class="foot-1">Help Center </div>
        </div>

        <div class="foot-1"> &#169; 2007-2022 Megashop.com</div>
        <img src="visa.png" alt="" class="img">
        <img src="cashdelivery.png" alt="" class="img">
        <img src="mastercard.png" alt="" class="img">
        <img src="paytm.png" alt="" class="img">
        <img src="rupay.png" alt="" class="img">
    </footer>
    <script src="https://kit.fontawesome.com/a076d05399.js"></script>
</body>

</html>
