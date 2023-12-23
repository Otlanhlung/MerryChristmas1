<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./publics/css/style.css">
    <link rel="shortcut icon" href="./publics/images/nvc_1.jpg" type="image/x-icon">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css" integrity="sha512-MV7K8+y+gLIBoVD59lQIYicR65iaqukzvf/nwasF0nqhPay5w/9lJmVM2hMDcnK1OnMGCdVK+iQrJ7lzPJQd1w==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <title>Merry Christmas </title>
</head>
<body>
    <div class="container">
        <div class="boxcontainer">
            <div class="image">
                <img src="./publics/images/gianginh2.png" alt="">
            </div>
            <div class="text-happybirthday">
                <img src="./publics/images/mery.png" alt="">
            </div>
            <div class="cake">
                <img src="./publics/images/caygiangsinh.png" alt="">
            </div>
            <div class="box-balloon">
                <div class="balloon-item1">
                    <img src="./publics/images/phaigs.png" alt="">
                </div>
                <div class="balloon-item1">
                    <img src="./publics/images/phaigs.png" alt="">
                </div>
            </div>
            <div class="box-cloud">
                <div class="cloud">
                    <img src="./publics/images/cloud.png" alt="">
                </div>
                <div class="cloud">
                    <img src="./publics/images/cloud.png" alt="">
                </div>
            </div>
            <div class="box-firework">
                <div class="firework">
                    <img src="./publics/images/firework.png" alt="">
                    <img src="./publics/images/firework1.png" alt="" id="firework1">
                </div>
                <div class="firework">
                    <img src="./publics/images/firework.png" alt="">
                    <img src="./publics/images/firework1.png" alt="" id="firework1">
                </div>
            </div>
            <div class="paperCannons">
                <img src="./publics/images/paperCannons1.png" alt="">
            </div>
            <div class="box-giftbox">
                <img src="./publics/images/giftbox.png" alt="">
                <img src="./publics/images/giftbox.png" alt="">
                <img src="./publics/images/giftbox.png" alt="">
                <img src="./publics/images/giftbox.png" alt="">
                <img src="./publics/images/giftbox.png" alt="">
                <img src="./publics/images/giftbox.png" alt="">
            </div>
            <div class="mail">
                <i class="fa-regular fa-envelope"></i>
            </div>
            <div class="boxcute">
                <div class="cute1">
                    <img src="./publics/images/cute.png" alt="">
                </div>
                <div class="cute2">
                    <img src="./publics/images/cute.png" alt="">
                </div>
            </div>
        </div>
        <div class="boxMail">
            <i class="fa-solid fa-xmark"></i>
            <div class="boxMail-container">
                <div class="card1">
                    <div class="userImg">
                        <img src="./publics/images/anhly2.jpg" alt="">
                    </div>
                    <h3>Merry Christmas</h3>
                    <div class="imageCute">
                        <img src="./publics/images/cute1.png" alt="">
                    </div>
                </div>
                <div class="card2">
                    <div class="card2-content">
                        <h3>Merry Christmas chị Ly Thỏ !</h3>
                        <h2>Chúc chị có một mùa Giáng sinh an lành, hạnh phúc, có những giây phút thật đáng nhớ, thật trọn vẹn  ^_^</h2>
                         <div class="imageCute2">
                            <img src="./publics/images/anhly1.jpg" alt="">
                         </div>
                         <div class="imageCute3">
                            <img src="./publics/images/anhly3.jpg" alt="" width="100%">
                         </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</body>
    <script>
        document.addEventListener('mousemove', function(e){
            let body = document.querySelector('body');
            let heart = document.createElement('span');
            let x = e.offsetX;
            let y = e.offsetY;
            heart.style.left = x+'px';
            heart.style.top = y+'px';

            let size = Math.random() * 10;
            heart.style.width = 4 * size+'px';
            heart.style.height = 4 * size+'px';


            let transformValue = Math.random() * 360;
            heart.style.transform = 'rotate('+ transformValue +'deg)';

            body.appendChild(heart);

            setTimeout(function(){
                heart.remove();
            },1000)
        })


        let mailBox = document.querySelector('.mail')
        let boxmail = document.querySelector('.boxMail')
        var close = document.querySelector('.fa-xmark')
        mailBox.onclick = function(){
            mailBox.classList.toggle('active')
            boxmail.classList.add('active')
        }

        close.addEventListener('click', function(){
            boxmail.classList.remove('active')
        })
    </script>
</html>
