Keyframes and animations module.
Code for module:
Index.html -
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="fun.css">
    <title>Document</title>
</head>
<body>
    <div class="box"></div>
</body>
</html>

Css code -
.box {
    background-color: #000;
    width: 150px;
    height: 0;
    margin: 25px;
    animation-name: growing;
    animation-duration: 2s;
    animation-timing-function: ease-in-out;
    animation-fill-mode: forwards;
    animation-iteration-count: infinite;
    animation-direction: alternate;
}

@keyframes growing {
    from {
        height: 0;
        }
    to {
        height: 150px;
    }
}

Following on from the lesson I am using this workspace to complete the challenge.
Make a ball jump up and down. It should go from top 0px to top 100px. One animation cycle should take half of a second and the animation should run infinitely. Name your keyframe jump. In the hint tab, you'll find a link to boilerplate files to help get you started.
Jump solution
@keyframes jump {
  0%   {transform: translate3d(0,0,0) scale3d(1,1,1);}
  40%  {transform: translate3d(0,30%,0) scale3d(.7,1.5,1);}
  100% {transform: translate3d(0,100%,0) scale3d(1.5,.7,1);}
}


Now the challenge has been completed I am using this workspace to work on the MOve, scale and spin lesson. I have cleared the workspace of code used previously and beginning fresh.
Challenge 2 has an unexpected outcome of flying in circles around the screen instead of rotating in one spot. Will keep just incase I want to do that again later on.
Code that produced the result:
img {
    margin: 50px;
    transition: transform 1s ease;
}

img:hover {
    transform: scale(2);
}

.challenge2 {
    animation-name: spin;
    animation-duration: 3s;
    animation-iteration-count: infinite;



}

@keyframes spin {
    from {
        transform: rotate(0deg)
    }
    to {
        transform: rotate(359deg)
    }

}

Moving on to challenge 3.