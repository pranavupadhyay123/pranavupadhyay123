<svg fill="none" viewBox="0 0 800 400" width="800" height="400" xmlns="http://www.w3.org/2000/svg">
	<foreignObject width="100%" height="100%">
		<div xmlns="http://www.w3.org/1999/xhtml">
            <style>
            *, *::after, *::before {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            user-select: none;
            transform-style: preserve-3d;
            -webkit-tap-highlight-color: transparent;
            }
            /* Generic */
            body {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 100%;
            height: 100vh;
            overflow: hidden;
            cursor: pointer;
            background-image: radial-gradient(circle, #171424, black);
            }
            .face {
            position: absolute;
            }
            /***************/
            .house {
            position: absolute;
            width: 28vw;
            height: 28vw;
            transform: perspective(90vw) rotateX(75deg) rotateZ(45deg) translateZ(-9vw);
            }
            .h-shadow {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            box-shadow: 1.5vw -3vw 3vw black, 1.5vw 0.5vw 1.5vw black;
            }
            .h-lights {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translateX(-50%) translateY(-50%);
            width: 45vw;
            height: 45vw;
            }
            .h-light {
            position: absolute;
            }
            .h-light:nth-of-type(1) {
            bottom: 5vw;
            right: 0;
            width: 14vw;
            height: 14vw;
            border-radius: 50%;
            background-image: radial-gradient(#1b182a, transparent);
            filter: blur(1vw);
            }
            .h-light:nth-of-type(2) {
            bottom: 18vw;
            right: -1vw;
            width: 2vw;
            height: 12vw;
            border-radius: 50%;
            transform: rotateZ(-50deg);
            background-image: radial-gradient(rgba(81, 137, 251, 0.45) 50%, rgba(40, 125, 210, 0.45), transparent);
            box-shadow: -1vw -1vw 2vw 1vw rgba(131, 171, 252, 0.1);
            filter: blur(1vw);
            }
            .h-light:nth-of-type(3) {
            bottom: -2vw;
            right: 17vw;
            width: 5vw;
            height: 12vw;
            border-radius: 50%;
            transform: rotateZ(-50deg);
            background-image: radial-gradient(rgba(81, 137, 251, 0.5) 50%, rgba(40, 125, 210, 0.5), transparent);
            filter: blur(2vw);
            }
            .h-light:nth-of-type(3)::before, .h-light:nth-of-type(3)::after {
            content: "";
            position: absolute;
            width: 200%;
            top: -6vw;
            height: 400%;
            background-image: linear-gradient(to bottom, rgba(40, 125, 210, 0.1), rgba(81, 137, 251, 0.1), transparent);
            border-top-left-radius: 10vw;
            border-top-right-radius: 10vw;
            filter: blur(1.5vw);
            }
            .h-light:nth-of-type(3)::before {
            right: -50%;
            transform-origin: top right;
            transform: rotateZ(15deg);
            box-shadow: -2vw -2vw 0 rgba(81, 137, 251, 0.075);
            }
            .h-light:nth-of-type(3)::after {
            left: -50%;
            transform-origin: top left;
            transform: rotateZ(-15deg);
            box-shadow: 2vw -2vw 0 rgba(81, 137, 251, 0.075);
            }
            .h-light:nth-of-type(4) {
            bottom: 5vw;
            left: 8vw;
            width: 28vw;
            height: 4vw;
            transform-origin: top left;
            transform: skewX(58deg);
            background-image: linear-gradient(to right, rgba(81, 137, 251, 0.075) 10%, transparent 25%, transparent, rgba(0, 0, 0, 0.15));
            filter: blur(0.25vw);
            }
            .h-light:nth-of-type(6) {
            bottom: 14vw;
            right: 2vw;
            width: 8vw;
            height: 16vw;
            transform-origin: bottom left;
            transform: skewY(49deg);
            background-image: linear-gradient(to left, rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.7));
            filter: blur(0.35vw);
            }
            /***************/
            /***************/
            .alt {
            position: absolute;
            left: 0;
            top: 0;
            width: 27vw;
            height: 27vw;
            }
            .alt__front {
            width: 27vw;
            height: 0.5vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(26.5vw);
            }
            .alt__back {
            width: 27vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-27vw) translateY(-0.5vw);
            }
            .alt__right {
            width: 27vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(27vw) translateX(-27vw) translateY(-0.5vw);
            }
            .alt__left {
            width: 27vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-0.5vw);
            }
            .alt__top {
            width: 27vw;
            height: 27vw;
            transform-origin: top left;
            transform: translateZ(0.5vw);
            }
            .alt__bottom {
            width: 27vw;
            height: 27vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-27vw);
            }
            .alt__front {
            background-color: #9E99C1;
            }
            .alt__back {
            background-color: #383358;
            }
            .alt__right {
            background-color: #383358;
            }
            .alt__left {
            background-color: #FBFAFE;
            }
            .alt__top {
            background-image: linear-gradient(to bottom, #0b0c1f, #383358, #9E99C1);
            }
            .alt__top .light:nth-of-type(1) {
            position: absolute;
            height: 100%;
            width: 100%;
            background-image: linear-gradient(to bottom, rgba(20, 61, 103, 0.75), rgba(81, 137, 251, 0.75), transparent);
            }
            .alt__top .light:nth-of-type(2) {
            position: absolute;
            left: 4vw;
            height: 100%;
            width: 6vw;
            background-image: linear-gradient(to bottom, transparent 20%, rgba(40, 125, 210, 0.75), rgba(81, 137, 251, 0.25) 80%);
            filter: blur(0.1vw);
            }
            .alt__top .light:nth-of-type(3) {
            position: absolute;
            bottom: 10vw;
            left: 5vw;
            width: 6vw;
            height: 3vw;
            border-radius: 50%;
            transform: rotateZ(42deg);
            background-image: radial-gradient(rgba(131, 171, 252, 0.75) 50%, rgba(32, 99, 167, 0.75));
            filter: blur(0.55vw);
            }
            .alt__top .light:nth-of-type(4) {
            position: absolute;
            bottom: 7vw;
            left: 4vw;
            width: 8.5vw;
            height: 2vw;
            border-radius: 50%;
            transform: rotateZ(40deg);
            background-image: radial-gradient(rgba(131, 171, 252, 0.75) 50%, rgba(32, 99, 167, 0.75));
            filter: blur(0.55vw);
            }
            .alt__top .light:nth-of-type(5) {
            position: absolute;
            bottom: 3.5vw;
            left: 4.5vw;
            width: 6vw;
            height: 2vw;
            border-radius: 50%;
            transform: rotateZ(40deg);
            background-image: radial-gradient(rgba(141, 178, 252, 0.75) 50%, rgba(32, 99, 167, 0.75));
            filter: blur(0.75vw);
            }
            .alt__top .light:nth-of-type(6) {
            position: absolute;
            bottom: 3vw;
            left: 0.5vw;
            width: 4vw;
            height: 2vw;
            border-radius: 50%;
            transform: rotateZ(40deg);
            background-image: radial-gradient(rgba(141, 178, 252, 0.75) 50%, rgba(32, 99, 167, 0.75));
            filter: blur(0.35vw);
            }
            .alt__top .light:nth-of-type(7) {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to right, black, #5189fb 10%, transparent 20%);
            }
            .alt__top .light:nth-of-type(7)::before {
            content: "";
            position: absolute;
            width: 20%;
            height: 100%;
            background-image: linear-gradient(to right, rgba(5, 70, 199, 0.6), transparent 60%);
            }
            .alt__top .light:nth-of-type(7)::after {
            content: "";
            position: absolute;
            width: 100%;
            height: 20%;
            background-image: linear-gradient(to bottom, rgba(6, 78, 224, 0.5), transparent 60%);
            }
            .alt__top .light:nth-of-type(8) {
            position: absolute;
            bottom: 5vw;
            left: 10vw;
            width: 6vw;
            height: 4vw;
            border-radius: 50%;
            transform: rotateZ(40deg);
            background-image: radial-gradient(rgba(255, 255, 255, 0.1) 50%, rgba(128, 121, 174, 0.1));
            filter: blur(0.8vw);
            }
            .alt__bottom {
            background-color: #383358;
            }
            .alb {
            position: absolute;
            left: 0;
            bottom: 0;
            width: 27vw;
            height: 1vw;
            }
            .alb__front {
            width: 27vw;
            height: 2vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(-1vw);
            }
            .alb__back {
            width: 27vw;
            height: 2vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-27vw) translateY(-2vw);
            }
            .alb__right {
            width: 1vw;
            height: 2vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(27vw) translateX(-1vw) translateY(-2vw);
            }
            .alb__left {
            width: 1vw;
            height: 2vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-2vw);
            }
            .alb__top {
            width: 27vw;
            height: 1vw;
            transform-origin: top left;
            transform: translateZ(2vw);
            }
            .alb__bottom {
            width: 27vw;
            height: 1vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-27vw);
            }
            .alb__front {
            background-image: linear-gradient(to right, #9E99C1 40%, #8f89b7);
            }
            .alb__back {
            background-color: #383358;
            }
            .alb__right {
            background-color: #383358;
            }
            .alb__left {
            background-color: #FBFAFE;
            }
            .alb__top {
            background-image: linear-gradient(to right, #FBFAFE 40%, #eae5fa);
            }
            .alb__bottom {
            background-color: #383358;
            }
            .arb {
            position: absolute;
            right: 0;
            bottom: 0;
            width: 1vw;
            height: 28vw;
            }
            .arb__front {
            width: 1vw;
            height: 2vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(26vw);
            }
            .arb__back {
            width: 1vw;
            height: 2vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-1vw) translateY(-2vw);
            }
            .arb__right {
            width: 28vw;
            height: 2vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(1vw) translateX(-28vw) translateY(-2vw);
            }
            .arb__left {
            width: 28vw;
            height: 2vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-2vw);
            }
            .arb__top {
            width: 1vw;
            height: 28vw;
            transform-origin: top left;
            transform: translateZ(2vw);
            }
            .arb__bottom {
            width: 1vw;
            height: 28vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-1vw);
            }
            .arb__front {
            background-color: #8f89b7;
            }
            .arb__back {
            background-color: #383358;
            }
            .arb__right {
            background-image: linear-gradient(to right, #282347 40%, #0f0e17);
            }
            .arb__left {
            background-color: #9E99C1;
            }
            .arb__top {
            background-image: linear-gradient(to top, #FBFAFE, #3b3469 25%, #2e2a48 75%, #9E99C1);
            }
            .arb__top::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 30%;
            top: 0;
            background-image: linear-gradient(to bottom, transparent, rgba(81, 137, 251, 0.85), transparent);
            }
            .arb__bottom {
            background-color: #383358;
            }
            /***************/
            /***************/
            .blt {
            position: absolute;
            left: 0;
            top: 0;
            width: 1vw;
            height: 27vw;
            transform: translateZ(0.5vw);
            }
            .blt__front {
            width: 1vw;
            height: 20vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(7vw);
            }
            .blt__back {
            width: 1vw;
            height: 20vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-1vw) translateY(-20vw);
            }
            .blt__right {
            width: 27vw;
            height: 20vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(1vw) translateX(-27vw) translateY(-20vw);
            }
            .blt__left {
            width: 27vw;
            height: 20vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-20vw);
            }
            .blt__top {
            width: 1vw;
            height: 27vw;
            transform-origin: top left;
            transform: translateZ(20vw);
            }
            .blt__bottom {
            width: 1vw;
            height: 27vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-1vw);
            }
            .blt__front {
            background-image: linear-gradient(to bottom, #383358, #9E99C1);
            }
            .blt__back {
            background-color: #383358;
            }
            .blt__right {
            background-image: linear-gradient(to bottom, #151225, #383358, #383358 90%, #242040);
            }
            .blt__right::before {
            content: "";
            position: absolute;
            bottom: 0;
            width: 100%;
            height: 0.75vw;
            background-image: linear-gradient(to bottom, #8f89b7, #287dd2);
            border-top: 0.1vw solid #282347;
            border-bottom: 0.1vw solid #282347;
            }
            .blt__right::after {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(6, 78, 224, 0.35), transparent 30%, transparent 70%, rgba(40, 125, 210, 0.35));
            }
            .blt__left {
            background-color: #FBFAFE;
            }
            .blt__bottom {
            background-color: #383358;
            }
            .blt2 {
            position: absolute;
            left: 0;
            top: 0;
            width: 2vw;
            height: 27vw;
            transform: translateZ(20.5vw);
            }
            .blt2__front {
            width: 2vw;
            height: 0.75vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(26.25vw);
            }
            .blt2__back {
            width: 2vw;
            height: 0.75vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-2vw) translateY(-0.75vw);
            }
            .blt2__right {
            width: 27vw;
            height: 0.75vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(2vw) translateX(-27vw) translateY(-0.75vw);
            }
            .blt2__left {
            width: 27vw;
            height: 0.75vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-0.75vw);
            }
            .blt2__top {
            width: 2vw;
            height: 27vw;
            transform-origin: top left;
            transform: translateZ(0.75vw);
            }
            .blt2__bottom {
            width: 2vw;
            height: 27vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-2vw);
            }
            .blt2__front {
            background-color: #383358;
            }
            .blt2__back {
            background-color: #383358;
            }
            .blt2__right {
            background-image: linear-gradient(to right, #8f89b7, #9E99C1, #7169a4);
            }
            .blt2__right::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            bottom: 0;
            border-bottom: 0.1vw solid rgba(251, 250, 254, 0.75);
            background-image: linear-gradient(to top, rgba(81, 137, 251, 0.35), transparent);
            }
            .blt2__left {
            background-color: #FBFAFE;
            }
            .blt2__top {
            background-image: linear-gradient(to top, #9E99C1, #FBFAFE);
            }
            .blt2__bottom {
            background-color: #383358;
            }
            .blb {
            position: absolute;
            left: 1vw;
            top: 0;
            width: 26vw;
            height: 1vw;
            transform: translateZ(0.5vw);
            }
            .blb__front {
            width: 26vw;
            height: 20vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(-19vw);
            }
            .blb__back {
            width: 26vw;
            height: 20vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-26vw) translateY(-20vw);
            }
            .blb__right {
            width: 1vw;
            height: 20vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(26vw) translateX(-1vw) translateY(-20vw);
            }
            .blb__left {
            width: 1vw;
            height: 20vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-20vw);
            }
            .blb__top {
            width: 26vw;
            height: 1vw;
            transform-origin: top left;
            transform: translateZ(20vw);
            }
            .blb__bottom {
            width: 26vw;
            height: 1vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-26vw);
            }
            .blb__front {
            background-image: linear-gradient(to bottom, #4b4572, #595388 20%, #4b4572);
            }
            .blb__front::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(40, 125, 210, 0.25), transparent 20%, transparent 80%, rgba(40, 125, 210, 0.5)), linear-gradient(to right, rgba(31, 33, 88, 0.35), transparent), linear-gradient(to bottom, rgba(31, 33, 88, 0.35), transparent), linear-gradient(to bottom, rgba(0, 0, 0, 0.5), transparent 20%, transparent 80%, rgba(40, 125, 210, 0.25));
            }
            .blb__front::after {
            content: "";
            position: absolute;
            bottom: 0;
            width: 100%;
            height: 0.75vw;
            background-image: linear-gradient(to bottom, #8f89b7, #287dd2);
            border-top: 0.1vw solid #282347;
            border-bottom: 0.1vw solid #282347;
            }
            .blb__back {
            background-color: #383358;
            }
            .blb__right {
            background-image: linear-gradient(to bottom, #151225, #0f0e17 80%, #151225);
            }
            .blb__bottom {
            background-color: #383358;
            }
            .blb2 {
            position: absolute;
            left: 2vw;
            top: 0;
            width: 25vw;
            height: 1vw;
            transform: translateZ(20.5vw);
            }
            .blb2__front {
            width: 25vw;
            height: 0.75vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(1.25vw);
            }
            .blb2__back {
            width: 25vw;
            height: 0.75vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-25vw) translateY(-0.75vw);
            }
            .blb2__right {
            width: 2vw;
            height: 0.75vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(25vw) translateX(-2vw) translateY(-0.75vw);
            }
            .blb2__left {
            width: 2vw;
            height: 0.75vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-0.75vw);
            }
            .blb2__top {
            width: 25vw;
            height: 2vw;
            transform-origin: top left;
            transform: translateZ(0.75vw);
            }
            .blb2__bottom {
            width: 25vw;
            height: 2vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-25vw);
            }
            .blb2__front {
            background-image: linear-gradient(to right, #7169a4, #9E99C1, #8f89b7);
            }
            .blb2__front::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            bottom: 0;
            border-bottom: 0.1vw solid rgba(251, 250, 254, 0.75);
            background-image: linear-gradient(to top, rgba(40, 125, 210, 0.25), transparent);
            }
            .blb2__back {
            background-color: #383358;
            }
            .blb2__right {
            background-color: #151225;
            }
            .blb2__left {
            background-color: #9E99C1;
            }
            .blb2__top {
            background-image: linear-gradient(to left, #9E99C1, #FBFAFE);
            }
            .blb2__bottom {
            background-color: #383358;
            }
            /***************/
            /***************/
            .bocina-l,
            .bocina-r {
            position: absolute;
            left: 1.5vw;
            bottom: 5.25vw;
            width: 0.75vw;
            height: 1.5vw;
            transform: translateZ(8vw);
            }
            .bocina-l__front,
            .bocina-r__front {
            width: 0.75vw;
            height: 6vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(-4.5vw);
            }
            .bocina-l__back,
            .bocina-r__back {
            width: 0.75vw;
            height: 6vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-0.75vw) translateY(-6vw);
            }
            .bocina-l__right,
            .bocina-r__right {
            width: 1.5vw;
            height: 6vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(0.75vw) translateX(-1.5vw) translateY(-6vw);
            }
            .bocina-l__left,
            .bocina-r__left {
            width: 1.5vw;
            height: 6vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-6vw);
            }
            .bocina-l__top,
            .bocina-r__top {
            width: 0.75vw;
            height: 1.5vw;
            transform-origin: top left;
            transform: translateZ(6vw);
            }
            .bocina-l__bottom,
            .bocina-r__bottom {
            width: 0.75vw;
            height: 1.5vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-0.75vw);
            }
            .bocina-l__right,
            .bocina-r__right {
            background-image: radial-gradient(black, black);
            }
            .bocina-l__top,
            .bocina-r__top {
            background-image: linear-gradient(to left, #d9d0f6, #9E99C1, #7169a4);
            }
            .bocina-l__bottom,
            .bocina-r__bottom {
            background-color: #383358;
            }
            .bocina-l__front {
            background-image: linear-gradient(to right, #5189fb, #595388 30%, #b7a5ed);
            }
            .bocina-l__back {
            background-image: linear-gradient(to right, #383358, #232038);
            }
            .bocina-l__back::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to right, rgba(81, 137, 251, 0.35) 65%, rgba(81, 137, 251, 0.95));
            }
            .bocina-l__left {
            background-color: #282347;
            }
            .bocina-l__left::before {
            content: "";
            position: absolute;
            top: -10%;
            left: 20%;
            width: 120%;
            height: 120%;
            background-image: linear-gradient(to left, rgba(7, 23, 39, 0.75), rgba(0, 0, 0, 0.75));
            filter: blur(0.5vw);
            }
            .bocina-r {
            top: 5.25vw;
            }
            .bocina-r__front {
            background-image: linear-gradient(to right, #383358, #0f0e17);
            }
            .bocina-r__front::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to left, rgba(81, 137, 251, 0.35) 65%, rgba(81, 137, 251, 0.95));
            }
            .bocina-r__back {
            background-image: linear-gradient(to right, #595388, #b7a5ed);
            }
            .bocina-r__left {
            background-color: #282347;
            }
            .bocina-r__left::before {
            content: "";
            position: absolute;
            top: -10%;
            left: -20%;
            width: 120%;
            height: 120%;
            background-image: linear-gradient(to right, rgba(7, 23, 39, 0.75), rgba(0, 0, 0, 0.75));
            filter: blur(0.5vw);
            }
            .repisa-t,
            .repisa-b {
            position: absolute;
            left: 1.5vw;
            top: 9vw;
            width: 1.5vw;
            height: 10vw;
            transform: translateZ(16vw);
            }
            .repisa-t__front,
            .repisa-b__front {
            width: 1.5vw;
            height: 0.25vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(9.75vw);
            }
            .repisa-t__back,
            .repisa-b__back {
            width: 1.5vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-1.5vw) translateY(-0.25vw);
            }
            .repisa-t__right,
            .repisa-b__right {
            width: 10vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(1.5vw) translateX(-10vw) translateY(-0.25vw);
            }
            .repisa-t__left,
            .repisa-b__left {
            width: 10vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-0.25vw);
            }
            .repisa-t__top,
            .repisa-b__top {
            width: 1.5vw;
            height: 10vw;
            transform-origin: top left;
            transform: translateZ(0.25vw);
            }
            .repisa-t__bottom,
            .repisa-b__bottom {
            width: 1.5vw;
            height: 10vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-1.5vw);
            }
            .repisa-t__front,
            .repisa-b__front {
            background-color: #9E99C1;
            }
            .repisa-t__back,
            .repisa-b__back {
            background-color: #FBFAFE;
            }
            .repisa-t__right,
            .repisa-b__right {
            background-color: #8079ae;
            }
            .repisa-t__left,
            .repisa-b__left {
            background-color: #FBFAFE;
            }
            .repisa-t__top,
            .repisa-b__top {
            background-color: #d9d0f6;
            }
            .repisa-t__top::before,
            .repisa-b__top::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to right, rgba(6, 78, 224, 0.75), transparent);
            }
            .repisa-t__bottom,
            .repisa-b__bottom {
            background-color: #383358;
            }
            .repisa-t__bottom::before,
            .repisa-b__bottom::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to right, rgba(6, 78, 224, 0.75), transparent);
            }
            .repisa-b {
            transform: translateZ(5vw);
            }
            .tv {
            position: absolute;
            left: 1.51vw;
            top: 8vw;
            width: 0.5vw;
            height: 12vw;
            transform: translateZ(8vw);
            }
            .tv__front {
            width: 0.5vw;
            height: 6vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(6vw);
            }
            .tv__back {
            width: 0.5vw;
            height: 6vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-0.5vw) translateY(-6vw);
            }
            .tv__right {
            width: 12vw;
            height: 6vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(0.5vw) translateX(-12vw) translateY(-6vw);
            }
            .tv__left {
            width: 12vw;
            height: 6vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-6vw);
            }
            .tv__top {
            width: 0.5vw;
            height: 12vw;
            transform-origin: top left;
            transform: translateZ(6vw);
            }
            .tv__bottom {
            width: 0.5vw;
            height: 12vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-0.5vw);
            }
            .tv__front {
            background-color: #0b0c1f;
            }
            .tv__back {
            background-color: #0b0c1f;
            }
            .tv__right {
            background-color: #9cbcfc;
            border: 0.125vw solid black;
            animation: pantalla-tv 0.25s infinite alternate;
            }
            .tv__right::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            box-shadow: 0.125vw 0.125vw 1vw rgba(81, 137, 251, 0.5), -0.125vw 0.125vw 1vw rgba(81, 137, 251, 0.5), 0.125vw -0.125vw 1vw rgba(81, 137, 251, 0.5), -0.125vw -0.125vw 1vw rgba(81, 137, 251, 0.5);
            background-image: url("coding.gif");
            background-size: cover;
            background-repeat: no-repeat;
            background-position: bottom;
            opacity: 0.8;
            }
            .tv__left {
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #0b0c1f;
            }
            .tv__left::before {
            content: "";
            position: absolute;
            width: 13vw;
            height: 7vw;
            background-image: radial-gradient(rgba(36, 112, 188, 0.95), rgba(56, 121, 250, 0.95));
            filter: blur(1.25vw);
            animation: luz-tv 0.25s infinite alternate;
            }
            .tv__top {
            background-color: #0b0c1f;
            }
            .tv__bottom {
            background-color: #0b0c1f;
            }
            .librero {
            position: absolute;
            left: 13vw;
            top: 1vw;
            width: 12vw;
            height: 0.5vw;
            transform: translateZ(7vw);
            }
            .librero__front {
            width: 12vw;
            height: 0.25vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(1.25vw);
            }
            .librero__back {
            width: 12vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-12vw) translateY(-0.25vw);
            }
            .librero__right {
            width: 1.5vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(12vw) translateX(-1.5vw) translateY(-0.25vw);
            }
            .librero__left {
            width: 1.5vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-0.25vw);
            }
            .librero__top {
            width: 12vw;
            height: 1.5vw;
            transform-origin: top left;
            transform: translateZ(0.25vw);
            }
            .librero__bottom {
            width: 12vw;
            height: 1.5vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-12vw);
            }
            .librero__front {
            background-color: #9E99C1;
            }
            .librero__back {
            background-color: #383358;
            }
            .librero__back::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 4vw;
            border-radius: 50%;
            background-image: radial-gradient(rgba(106, 154, 251, 0.7) 50%, rgba(32, 99, 167, 0.6), transparent);
            filter: blur(1.25vw);
            }
            .librero__right {
            background-color: #383358;
            }
            .librero__left {
            background-color: #9E99C1;
            }
            .librero__top {
            background-color: #d9d0f6;
            }
            .librero__top::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(31, 104, 249, 0.75), transparent);
            }
            .librero__bottom {
            background-color: #383358;
            }
            .librero__bottom::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(31, 104, 249, 0.75), transparent);
            }
            .libros {
            position: absolute;
            }
            .libro {
            position: absolute;
            top: 1vw;
            width: 0.5vw;
            height: 1vw;
            transform: translateZ(7.25vw);
            }
            .libro__front {
            width: 0.5vw;
            height: 1.5vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(-0.5vw);
            }
            .libro__back {
            width: 0.5vw;
            height: 1.5vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-0.5vw) translateY(-1.5vw);
            }
            .libro__right {
            width: 1vw;
            height: 1.5vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(0.5vw) translateX(-1vw) translateY(-1.5vw);
            }
            .libro__left {
            width: 1vw;
            height: 1.5vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-1.5vw);
            }
            .libro__top {
            width: 0.5vw;
            height: 1vw;
            transform-origin: top left;
            transform: translateZ(1.5vw);
            }
            .libro__bottom {
            width: 0.5vw;
            height: 1vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-0.5vw);
            }
            .libro__front {
            background-image: linear-gradient(to bottom, #9E99C1, #8079ae);
            }
            .libro__front::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(81, 137, 251, 0.4), transparent);
            }
            .libro__back {
            background-color: #FBFAFE;
            }
            .libro__right {
            background-color: #645c98;
            }
            .libro__right::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(81, 137, 251, 0.85), rgba(40, 125, 210, 0.35));
            }
            .libro__left {
            background-color: #9E99C1;
            }
            .libro__top {
            background-color: #d9d0f6;
            }
            .libro__top::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(81, 137, 251, 0.85), rgba(40, 125, 210, 0.35));
            }
            .libro__bottom {
            background-color: #554d85;
            }
            .libro:nth-of-type(1) {
            left: 16vw;
            transform-origin: left;
            transform: translateZ(7.25vw) rotateZ(-10deg);
            }
            .libro:nth-of-type(2) {
            left: 17vw;
            transform: translateZ(7.25vw) rotateZ(2deg);
            }
            .libro:nth-of-type(3) {
            left: 17.75vw;
            transform: translateZ(7.25vw) rotateZ(5deg);
            }
            .libro:nth-of-type(4) {
            left: 19vw;
            transform-origin: left;
            transform: translateZ(7.25vw) rotateZ(10deg);
            }
            .libro:nth-of-type(5) {
            left: 20vw;
            transform-origin: left;
            transform: translateZ(7.25vw) rotateZ(10deg);
            }
            .libro:nth-of-type(6) {
            left: 23vw;
            transform-origin: left;
            transform: translateZ(7.25vw) rotateY(-90deg);
            }
            .fotos {
            position: absolute;
            }
            .foto {
            position: absolute;
            width: 0.125vw;
            height: 2vw;
            left: 2vw;
            top: 11vw;
            transform: translateZ(5.26vw);
            }
            .foto__front {
            width: 0.125vw;
            height: 1.125vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(1.125vw);
            }
            .foto__back {
            width: 0.125vw;
            height: 1.125vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-0.125vw) translateY(-1.125vw);
            }
            .foto__right {
            width: 2.25vw;
            height: 1.125vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(0.125vw) translateX(-2.25vw) translateY(-1.125vw);
            }
            .foto__left {
            width: 2.25vw;
            height: 1.125vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-1.125vw);
            }
            .foto__top {
            width: 0.125vw;
            height: 2.25vw;
            transform-origin: top left;
            transform: translateZ(1.125vw);
            }
            .foto__bottom {
            width: 0.125vw;
            height: 2.25vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-0.125vw);
            }
            .foto__front {
            background-image: linear-gradient(to bottom, #9E99C1, #8079ae);
            }
            .foto__front::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(81, 137, 251, 0.4), transparent);
            }
            .foto__back {
            background-color: #FBFAFE;
            }
            .foto__right {
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #8f89b7;
            border: 0.15vw solid #1f2158;
            }
            .foto__right::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: repeating-linear-gradient(to bottom, #9E99C1 0.1vw, #b7a5ed 0.2vw);
            }
            .foto__left {
            background-color: #9E99C1;
            }
            .foto__top {
            background-color: #d9d0f6;
            }
            .foto__top::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(81, 137, 251, 0.85), rgba(40, 125, 210, 0.35));
            }
            .foto__bottom {
            background-color: #595388;
            }
            .foto__bottom::before {
            content: "";
            position: absolute;
            right: -100%;
            width: 400%;
            height: 100%;
            background-color: rgba(11, 12, 31, 0.75);
            filter: blur(0.15vw);
            }
            .foto:nth-of-type(1) {
            top: 10.5vw;
            transform: translateZ(5.26vw) rotateZ(5deg);
            }
            .foto:nth-of-type(2) {
            top: 15vw;
            transform: translateZ(5.26vw) rotateZ(-15deg);
            }
            .cajas {
            position: absolute;
            }
            .caja {
            position: absolute;
            width: 1vw;
            height: 1.5vw;
            left: 2vw;
            transform: translateZ(16.35vw);
            }
            .caja__front {
            width: 1vw;
            height: 0.75vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(0.75vw);
            }
            .caja__back {
            width: 1vw;
            height: 0.75vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-1vw) translateY(-0.75vw);
            }
            .caja__right {
            width: 1.5vw;
            height: 0.75vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(1vw) translateX(-1.5vw) translateY(-0.75vw);
            }
            .caja__left {
            width: 1.5vw;
            height: 0.75vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-0.75vw);
            }
            .caja__top {
            width: 1vw;
            height: 1.5vw;
            transform-origin: top left;
            transform: translateZ(0.75vw);
            }
            .caja__bottom {
            width: 1vw;
            height: 1.5vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-1vw);
            }
            .caja__front {
            background-image: linear-gradient(to bottom, #9E99C1, #8079ae);
            }
            .caja__front::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(81, 137, 251, 0.4), transparent);
            }
            .caja__back {
            background-color: #9E99C1;
            }
            .caja__right {
            background-color: #645c98;
            }
            .caja__right::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(81, 137, 251, 0.85), rgba(40, 125, 210, 0.35));
            }
            .caja__left {
            background-color: #9E99C1;
            }
            .caja__top {
            background-color: #d9d0f6;
            }
            .caja__top::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(81, 137, 251, 0.85), rgba(40, 125, 210, 0.35));
            }
            .caja__bottom {
            background-color: #595388;
            }
            .caja__bottom::before {
            content: "";
            position: absolute;
            right: -50%;
            width: 150%;
            height: 120%;
            background-color: rgba(31, 33, 88, 0.5);
            filter: blur(0.15vw);
            }
            .caja:nth-of-type(1) {
            top: 11.6vw;
            }
            .caja:nth-of-type(2) {
            top: 13.5vw;
            }
            .caja:nth-of-type(3) {
            top: 17vw;
            }
            .cuadro-l,
            .cuadro-r {
            position: absolute;
            left: 13vw;
            top: 1vw;
            width: 5vw;
            height: 0.5vw;
            transform: translateZ(10vw);
            }
            .cuadro-l__front,
            .cuadro-r__front {
            width: 5vw;
            height: 7vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(-6.75vw);
            }
            .cuadro-l__back,
            .cuadro-r__back {
            width: 5vw;
            height: 7vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-5vw) translateY(-7vw);
            }
            .cuadro-l__right,
            .cuadro-r__right {
            width: 0.25vw;
            height: 7vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(5vw) translateX(-0.25vw) translateY(-7vw);
            }
            .cuadro-l__left,
            .cuadro-r__left {
            width: 0.25vw;
            height: 7vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-7vw);
            }
            .cuadro-l__top,
            .cuadro-r__top {
            width: 5vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: translateZ(7vw);
            }
            .cuadro-l__bottom,
            .cuadro-r__bottom {
            width: 5vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-5vw);
            }
            .cuadro-l__front,
            .cuadro-r__front {
            background-repeat: no-repeat;
            background-size: contain;
            background-position: center;
            }
            .cuadro-l__back,
            .cuadro-r__back {
            background-color: #383358;
            box-shadow: 0.35vw 0.35vw 0.35vw rgba(81, 137, 251, 0.2), -0.35vw 0.35vw 0.35vw rgba(81, 137, 251, 0.2), -0.35vw -0.35vw 0.35vw rgba(81, 137, 251, 0.2), 0.35vw -0.35vw 0.35vw rgba(81, 137, 251, 0.2);
            }
            .cuadro-l__right,
            .cuadro-r__right {
            background-color: #383358;
            }
            .cuadro-l__left,
            .cuadro-r__left {
            background-color: #9E99C1;
            }
            .cuadro-l__top,
            .cuadro-r__top {
            background-color: #9E99C1;
            }
            .cuadro-l__bottom,
            .cuadro-r__bottom {
            background-color: #383358;
            }
            .cuadro-l__front {
            background-image: url("https://rawcdn.githack.com/ricardoolivaalonso/Codepen/43200238c3177b02a97423fa6cc23f8bfcc5c105/Room/cuadro-1.jpg");
            background-color: #D51E24;
            border: 1vw solid #D51E24;
            }
            .cuadro-l__front::before {
            content: "";
            position: absolute;
            top: -1vw;
            left: -1vw;
            width: 5vw;
            height: 7vw;
            background-origin: padding-box;
            background-image: linear-gradient(to bottom, rgba(40, 125, 210, 0.15), rgba(40, 125, 210, 0.15));
            }
            .cuadro-r {
            left: 20vw;
            }
            .cuadro-r__front {
            background-image: url("https://rawcdn.githack.com/ricardoolivaalonso/Codepen/43200238c3177b02a97423fa6cc23f8bfcc5c105/Room/cuadro-2.jpg");
            background-color: #0F1110;
            border: 0.5vw solid #0F1110;
            }
            .cuadro-r__front::before {
            content: "";
            position: absolute;
            top: -0.5vw;
            left: -0.5vw;
            width: 5vw;
            height: 7vw;
            background-origin: padding-box;
            background-image: linear-gradient(to bottom, rgba(40, 125, 210, 0.15), rgba(40, 125, 210, 0.15));
            }
            .puerta-c {
            position: absolute;
            left: 3vw;
            top: 1vw;
            width: 8vw;
            height: 0.5vw;
            transform: translateZ(0.5vw);
            }
            .puerta-c::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 200%;
            background-color: rgba(0, 0, 0, 0.65);
            filter: blur(0.5vw);
            }
            .puerta {
            position: absolute;
            left: 0.5vw;
            top: 0;
            width: 7vw;
            height: 0.5vw;
            }
            .puerta__front {
            width: 7vw;
            height: 16vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(-15.75vw);
            }
            .puerta__back {
            width: 7vw;
            height: 16vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-7vw) translateY(-16vw);
            }
            .puerta__right {
            width: 0.25vw;
            height: 16vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(7vw) translateX(-0.25vw) translateY(-16vw);
            }
            .puerta__left {
            width: 0.25vw;
            height: 16vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-16vw);
            }
            .puerta__top {
            width: 7vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: translateZ(16vw);
            }
            .puerta__bottom {
            width: 7vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-7vw);
            }
            .puerta__front {
            background-image: linear-gradient(to bottom, #0F1110, #121332);
            border: 0.125vw solid #5189fb;
            }
            .puerta__front::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: radial-gradient(transparent 50%, rgba(4, 61, 174, 0.25));
            box-shadow: 0.65vw 0.65vw 0.5vw rgba(81, 137, 251, 0.6), -0.65vw 0.65vw 0.5vw rgba(81, 137, 251, 0.6), -0.65vw -0.65vw 0.5vw rgba(81, 137, 251, 0.6), 0.65vw -0.65vw 0.5vw rgba(81, 137, 251, 0.6);
            }
            .puerta__front::after {
            content: "";
            position: absolute;
            top: 50%;
            right: 0.75vw;
            width: 1vw;
            height: 0.25vw;
            background-color: #9E99C1;
            box-shadow: 0.125vw 0.125vw 0.25vw rgba(81, 137, 251, 0.6), -0.125vw 0.125vw 0.25vw rgba(81, 137, 251, 0.6), -0.125vw -0.125vw 0.25vw rgba(81, 137, 251, 0.6), 0.125vw -0.125vw 0.25vw rgba(81, 137, 251, 0.6);
            }
            .puerta-l,
            .puerta-r {
            position: absolute;
            left: 0;
            top: 0;
            width: 0.5vw;
            height: 0.5vw;
            }
            .puerta-l__front,
            .puerta-r__front {
            width: 0.5vw;
            height: 16vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(-15.5vw);
            }
            .puerta-l__back,
            .puerta-r__back {
            width: 0.5vw;
            height: 16vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-0.5vw) translateY(-16vw);
            }
            .puerta-l__right,
            .puerta-r__right {
            width: 0.5vw;
            height: 16vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(0.5vw) translateX(-0.5vw) translateY(-16vw);
            }
            .puerta-l__left,
            .puerta-r__left {
            width: 0.5vw;
            height: 16vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-16vw);
            }
            .puerta-l__top,
            .puerta-r__top {
            width: 0.5vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: translateZ(16vw);
            }
            .puerta-l__bottom,
            .puerta-r__bottom {
            width: 0.5vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-0.5vw);
            }
            .puerta-l__front,
            .puerta-r__front {
            background-color: #121332;
            }
            .puerta-l__back,
            .puerta-r__back {
            background-color: #0b0c1f;
            }
            .puerta-l__right,
            .puerta-r__right {
            background-color: #0b0c1f;
            }
            .puerta-l__left,
            .puerta-r__left {
            background-color: #121332;
            }
            .puerta-l__bottom,
            .puerta-r__bottom {
            background-color: #0b0c1f;
            }
            .puerta-r {
            left: calc(100% - .5vw);
            }
            .puerta-t {
            left: 0;
            top: 0;
            width: 8vw;
            height: 0.5vw;
            transform: translateZ(16vw);
            }
            .puerta-t__front {
            width: 8vw;
            height: 0.5vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(0vw);
            }
            .puerta-t__back {
            width: 8vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-8vw) translateY(-0.5vw);
            }
            .puerta-t__right {
            width: 0.5vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(8vw) translateX(-0.5vw) translateY(-0.5vw);
            }
            .puerta-t__left {
            width: 0.5vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-0.5vw);
            }
            .puerta-t__top {
            width: 8vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: translateZ(0.5vw);
            }
            .puerta-t__bottom {
            width: 8vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-8vw);
            }
            .puerta-t__front {
            background-color: #121332;
            }
            .puerta-t__back {
            background-color: #0b0c1f;
            }
            .puerta-t__right {
            background-color: #0b0c1f;
            }
            .puerta-t__left {
            background-color: #121332;
            }
            .puerta-t__top {
            background-color: #1f2158;
            }
            .puerta-t__bottom {
            background-color: #0b0c1f;
            }
            .muro {
            position: absolute;
            left: 1vw;
            top: 6vw;
            width: 0.5vw;
            height: 16vw;
            transform: translateZ(0.51vw);
            }
            .muro__front {
            width: 0.5vw;
            height: 18vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(-2vw);
            }
            .muro__back {
            width: 0.5vw;
            height: 18vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-0.5vw) translateY(-18vw);
            }
            .muro__right {
            width: 16vw;
            height: 18vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(0.5vw) translateX(-16vw) translateY(-18vw);
            }
            .muro__left {
            width: 16vw;
            height: 18vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-18vw);
            }
            .muro__top {
            width: 0.5vw;
            height: 16vw;
            transform-origin: top left;
            transform: translateZ(18vw);
            }
            .muro__bottom {
            width: 0.5vw;
            height: 16vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-0.5vw);
            }
            .muro__front {
            background-color: #0b0c1f;
            }
            .muro__back {
            background-color: #0b0c1f;
            }
            .muro__right {
            display: flex;
            justify-content: center;
            background-image: radial-gradient(circle, #1f2158, #0b0c1f);
            overflow: hidden;
            }
            .muro__right::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(40, 125, 210, 0.25), transparent 30%, transparent 70%, rgba(40, 125, 210, 0.15));
            }
            .muro__right::after {
            content: "";
            position: absolute;
            bottom: 0;
            left: 5%;
            width: 90%;
            height: 25%;
            background-image: linear-gradient(to bottom, rgba(4, 5, 13, 0.75), rgba(4, 5, 13, 0.95));
            filter: blur(0.75vw);
            }
            .muro__left {
            background-color: #0b0c1f;
            box-shadow: 0.5vw 0.5vw 0.6vw rgba(81, 137, 251, 0.3), 0.5vw -0.5vw 0.6vw rgba(81, 137, 251, 0.3), -0.5vw 0.5vw 0.6vw rgba(81, 137, 251, 0.3), -0.5vw -0.5vw 0.6vw rgba(81, 137, 251, 0.3);
            }
            .muro__top {
            background-color: #0b0c1f;
            }
            .muro__top::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            bottom: 0;
            background-image: linear-gradient(to left, rgba(40, 125, 210, 0.5), rgba(81, 137, 251, 0.25));
            }
            .muro__bottom {
            background-color: #0b0c1f;
            }
            .muro__bottom::before {
            content: "";
            position: absolute;
            top: 0;
            right: 0;
            width: 5vw;
            height: 100%;
            background-image: linear-gradient(to left, #0b0c1f, transparent 50%);
            transform-origin: right bottom;
            transform: skewY(-20deg);
            filter: blur(0.25vw);
            }
            .sillon-c {
            position: absolute;
            right: 2vw;
            bottom: 6vw;
            width: 6vw;
            height: 16vw;
            transform: translateZ(0.5vw);
            }
            .sillon-c::before {
            content: "";
            position: absolute;
            top: -10%;
            left: -10%;
            width: 120%;
            height: 120%;
            background-color: rgba(11, 12, 31, 0.85);
            filter: blur(0.75vw);
            }
            .sillon-b {
            position: absolute;
            left: 0;
            top: 1vw;
            width: 6vw;
            height: 14vw;
            }
            .sillon-b__front {
            width: 6vw;
            height: 3vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(11vw);
            }
            .sillon-b__back {
            width: 6vw;
            height: 3vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-6vw) translateY(-3vw);
            }
            .sillon-b__right {
            width: 14vw;
            height: 3vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(6vw) translateX(-14vw) translateY(-3vw);
            }
            .sillon-b__left {
            width: 14vw;
            height: 3vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-3vw);
            }
            .sillon-b__top {
            width: 6vw;
            height: 14vw;
            transform-origin: top left;
            transform: translateZ(3vw);
            }
            .sillon-b__bottom {
            width: 6vw;
            height: 14vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-6vw);
            }
            .sillon-b__front {
            background-color: #121332;
            }
            .sillon-b__back {
            background-color: #0b0c1f;
            }
            .sillon-b__right {
            background-color: #0b0c1f;
            }
            .sillon-b__left {
            background-image: linear-gradient(to bottom, #121332, #0b0c1f);
            }
            .sillon-b__left::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to bottom, rgba(40, 125, 210, 0.1), transparent);
            }
            .sillon-b__top {
            background-image: linear-gradient(to right, #1f2158, #121332);
            border-left: 0.1vw solid rgba(158, 153, 193, 0.5);
            }
            .sillon-b__top::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to right, rgba(40, 125, 210, 0.25), transparent);
            }
            .sillon-b__bottom {
            background-color: #0b0c1f;
            }
            .sillon-l,
            .sillon-r {
            position: absolute;
            left: 0;
            bottom: 0;
            width: 6vw;
            height: 1vw;
            }
            .sillon-l__front,
            .sillon-r__front {
            width: 6vw;
            height: 4.5vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(-3.5vw);
            }
            .sillon-l__back,
            .sillon-r__back {
            width: 6vw;
            height: 4.5vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-6vw) translateY(-4.5vw);
            }
            .sillon-l__right,
            .sillon-r__right {
            width: 1vw;
            height: 4.5vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(6vw) translateX(-1vw) translateY(-4.5vw);
            }
            .sillon-l__left,
            .sillon-r__left {
            width: 1vw;
            height: 4.5vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-4.5vw);
            }
            .sillon-l__top,
            .sillon-r__top {
            width: 6vw;
            height: 1vw;
            transform-origin: top left;
            transform: translateZ(4.5vw);
            }
            .sillon-l__bottom,
            .sillon-r__bottom {
            width: 6vw;
            height: 1vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-6vw);
            }
            .sillon-l__front,
            .sillon-r__front {
            background-image: linear-gradient(to bottom, #121332, #0b0c1f);
            }
            .sillon-l__back,
            .sillon-r__back {
            background-color: #0b0c1f;
            }
            .sillon-l__right,
            .sillon-r__right {
            background-image: linear-gradient(to bottom, #0b0c1f, black);
            }
            .sillon-l__left,
            .sillon-r__left {
            background-image: linear-gradient(to bottom, #121332, #0b0c1f);
            }
            .sillon-l__top,
            .sillon-r__top {
            background-image: linear-gradient(to right, #1f2158, #0f102b);
            border-bottom: 0.1vw solid rgba(158, 153, 193, 0.5);
            }
            .sillon-l__top::before,
            .sillon-r__top::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to right, rgba(40, 125, 210, 0.75), transparent);
            }
            .sillon-l__bottom,
            .sillon-r__bottom {
            background-color: #0b0c1f;
            }
            .sillon-r {
            top: 0;
            }
            .sillon-t {
            position: absolute;
            right: 0;
            top: 1vw;
            width: 1vw;
            height: 1vw;
            transform-origin: right;
            transform: rotateY(7deg);
            }
            .sillon-t__front {
            width: 1vw;
            height: 6.5vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(7.5vw);
            }
            .sillon-t__back {
            width: 1vw;
            height: 6.5vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-1vw) translateY(-6.5vw);
            }
            .sillon-t__right {
            width: 14vw;
            height: 6.5vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(1vw) translateX(-14vw) translateY(-6.5vw);
            }
            .sillon-t__left {
            width: 14vw;
            height: 6.5vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-6.5vw);
            }
            .sillon-t__top {
            width: 1vw;
            height: 14vw;
            transform-origin: top left;
            transform: translateZ(6.5vw);
            }
            .sillon-t__bottom {
            width: 1vw;
            height: 14vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-1vw);
            }
            .sillon-t__front {
            background-image: linear-gradient(to bottom, #0b0c1f, #070814);
            }
            .sillon-t__back {
            background-image: linear-gradient(to bottom, #0b0c1f, #0b0c1f);
            }
            .sillon-t__right {
            background-image: linear-gradient(to bottom, #0b0c1f, black);
            }
            .sillon-t__left {
            background-color: #121332;
            }
            .sillon-t__top {
            background-image: linear-gradient(to right, #1f2158, #0f102b);
            border-bottom: 0.1vw solid rgba(158, 153, 193, 0.5);
            }
            .sillon-t__top::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(to right, rgba(40, 125, 210, 0.5), transparent);
            }
            .sillon-t__bottom {
            background-color: #0b0c1f;
            }
            .mesa-c {
            position: absolute;
            left: 7vw;
            top: 9.5vw;
            width: 10vw;
            height: 9vw;
            transform: translateZ(0.5vw);
            }
            .mesa-shadow {
            position: absolute;
            width: 100%;
            height: 100%;
            border-radius: 10%;
            background-color: rgba(11, 12, 31, 0.95);
            filter: blur(1vw);
            transform: translateZ(0);
            }
            .mesa {
            position: absolute;
            left: 0;
            top: 0;
            width: 10vw;
            height: 9vw;
            transform: translateZ(2vw);
            }
            .mesa__front {
            width: 10vw;
            height: 0.5vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(8.5vw);
            }
            .mesa__back {
            width: 10vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-10vw) translateY(-0.5vw);
            }
            .mesa__right {
            width: 9vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(10vw) translateX(-9vw) translateY(-0.5vw);
            }
            .mesa__left {
            width: 9vw;
            height: 0.5vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-0.5vw);
            }
            .mesa__top {
            width: 10vw;
            height: 9vw;
            transform-origin: top left;
            transform: translateZ(0.5vw);
            }
            .mesa__bottom {
            width: 10vw;
            height: 9vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-10vw);
            }
            .mesa__front {
            background-image: linear-gradient(to right, #0b0c1f, black);
            }
            .mesa__front::before {
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-image: linear-gradient(45deg, rgba(81, 137, 251, 0.125), rgba(180, 205, 253, 0.25), transparent 55%);
            }
            .mesa__back {
            background-color: #0b0c1f;
            }
            .mesa__right {
            background-color: black;
            }
            .mesa__left {
            background-color: #121332;
            }
            .mesa__top {
            background-image: linear-gradient(45deg, #0e0f27, #04050d);
            overflow: hidden;
            }
            .mesa__top::before {
            content: "";
            position: absolute;
            bottom: 0;
            width: 50%;
            height: 50%;
            background-image: linear-gradient(45deg, rgba(81, 137, 251, 0.5), rgba(251, 250, 254, 0.125) 50%, transparent 55%);
            filter: blur(0.5vw);
            }
            .mesa__top::after {
            content: "";
            position: absolute;
            left: 2vw;
            top: 2vw;
            width: 20%;
            height: 50%;
            border-radius: 50%;
            background-color: rgba(40, 125, 210, 0.079);
            transform: rotateZ(-40deg);
            filter: blur(0.75vw);
            }
            .mesa__bottom {
            background-color: #0b0c1f;
            }
            .mesa-p {
            position: absolute;
            width: 0.25vw;
            height: 0.25vw;
            }
            .mesa-p__front {
            width: 0.25vw;
            height: 1.75vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(-1.5vw);
            }
            .mesa-p__back {
            width: 0.25vw;
            height: 1.75vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-0.25vw) translateY(-1.75vw);
            }
            .mesa-p__right {
            width: 0.25vw;
            height: 1.75vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(0.25vw) translateX(-0.25vw) translateY(-1.75vw);
            }
            .mesa-p__left {
            width: 0.25vw;
            height: 1.75vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-1.75vw);
            }
            .mesa-p__top {
            width: 0.25vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: translateZ(1.75vw);
            }
            .mesa-p__bottom {
            width: 0.25vw;
            height: 0.25vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-0.25vw);
            }
            .mesa-p__front {
            background-color: #0b0c1f;
            }
            .mesa-p__back {
            background-color: #0b0c1f;
            }
            .mesa-p__right {
            background-color: black;
            }
            .mesa-p__left {
            background-color: #121332;
            }
            .mesa-p__top {
            background-color: #1f2158;
            }
            .mesa-p__bottom {
            background-color: #0b0c1f;
            }
            .mesa-p__bottom::before {
            content: "";
            position: absolute;
            width: 600%;
            height: 200%;
            top: 0;
            right: 0;
            border-radius: 10%;
            transform: translateZ(-0.1vw);
            background-color: rgba(0, 0, 0, 0.75);
            filter: blur(0.35vw);
            }
            .mesa-p:nth-of-type(1) {
            left: 0.5vw;
            top: 0.5vw;
            }
            .mesa-p:nth-of-type(2) {
            right: 0.5vw;
            top: 0.5vw;
            }
            .mesa-p:nth-of-type(3) {
            left: 0.5vw;
            bottom: 0.5vw;
            }
            .mesa-p:nth-of-type(4) {
            right: 0.5vw;
            bottom: 0.5vw;
            }
            .tablet {
            position: absolute;
            left: 13vw;
            top: 12vw;
            width: 2vw;
            height: 2.5vw;
            transform: translateZ(3.01vw) rotateZ(15deg);
            }
            .tablet__front {
            width: 2vw;
            height: 0.125vw;
            transform-origin: bottom left;
            transform: rotateX(-90deg) translateZ(2.375vw);
            }
            .tablet__back {
            width: 2vw;
            height: 0.125vw;
            transform-origin: top left;
            transform: rotateX(-90deg) rotateY(180deg) translateX(-2vw) translateY(-0.125vw);
            }
            .tablet__right {
            width: 2.5vw;
            height: 0.125vw;
            transform-origin: top left;
            transform: rotateY(90deg) rotateZ(-90deg) translateZ(2vw) translateX(-2.5vw) translateY(-0.125vw);
            }
            .tablet__left {
            width: 2.5vw;
            height: 0.125vw;
            transform-origin: top left;
            transform: rotateY(-90deg) rotateZ(90deg) translateY(-0.125vw);
            }
            .tablet__top {
            width: 2vw;
            height: 2.5vw;
            transform-origin: top left;
            transform: translateZ(0.125vw);
            }
            .tablet__bottom {
            width: 2vw;
            height: 2.5vw;
            transform-origin: top left;
            transform: rotateY(180deg) translateX(-2vw);
            }
            .tablet__front {
            background-color: #8079ae;
            }
            .tablet__back {
            background-color: #383358;
            }
            .tablet__right {
            background-color: #383358;
            }
            .tablet__left {
            background-color: #9E99C1;
            }
            .tablet__top {
            background-color: #83abfc;
            border: 0.2vw solid rgba(81, 137, 251, 0.25);
            animation: pantalla-tablet 0.25s infinite;
            }
            .tablet__bottom {
            background-color: black;
            box-shadow: 0.25vw 0.25vw 0.5vw rgba(24, 74, 124, 0.75), -0.25vw 0.25vw 0.5vw rgba(24, 74, 124, 0.75), -0.25vw -0.25vw 0.5vw rgba(24, 74, 124, 0.75), 0.25vw -0.25vw 0.5vw rgba(24, 74, 124, 0.75);
            }
            /**********************/
            /**********************/
            @keyframes pantalla-tablet {
            from {
                background-color: #6a9afb;
            }
            }
            @keyframes pantalla-tv {
            from {
                background-color: #6a9afb;
                box-shadow: 0.125vw 0.125vw 0vw rgba(81, 137, 251, 0), -0.125vw 0.125vw 0vw rgba(81, 137, 251, 0), 0.125vw -0.125vw 0vw rgba(81, 137, 251, 0), -0.125vw -0.125vw 0vw rgba(81, 137, 251, 0);
            }
            }
            @keyframes luz-tv {
            from {
                background-image: radial-gradient(rgba(36, 112, 188, 0.8), rgba(56, 121, 250, 0.8));
            }
            }
        </style>
<div class="house" id="h">
    <div class="h-lights">
      <div class="h-light"></div>
      <div class="h-light"></div>
      <div class="h-light"></div>
      <div class="h-light"></div>
      <div class="h-light"></div>
      <div class="h-light"></div>
    </div>
    <div class="h-shadow"></div>
    <div class="alt">
      <div class="alt__front face"> </div>
      <div class="alt__back face"> </div>
      <div class="alt__right face"> </div>
      <div class="alt__left face"> </div>
      <div class="alt__top face">
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
      </div>
      <div class="alt__bottom face"> </div>
    </div>
    <div class="alb">
      <div class="alb__front face"> </div>
      <div class="alb__back face"> </div>
      <div class="alb__right face"> </div>
      <div class="alb__left face"> </div>
      <div class="alb__top face"> </div>
      <div class="alb__bottom face"> </div>
    </div>
    <div class="arb">
      <div class="arb__front face"> </div>
      <div class="arb__back face"> </div>
      <div class="arb__right face"> </div>
      <div class="arb__left face"> </div>
      <div class="arb__top face"> </div>
      <div class="arb__bottom face"> </div>
    </div>
    <div class="blt">
      <div class="blt__front face"> </div>
      <div class="blt__back face"> </div>
      <div class="blt__right face"> </div>
      <div class="blt__left face"> </div>
      <div class="blt__top face"> </div>
      <div class="blt__bottom face"> </div>
    </div>
    <div class="blt2">
      <div class="blt2__front face"> </div>
      <div class="blt2__back face"> </div>
      <div class="blt2__right face"> </div>
      <div class="blt2__left face"> </div>
      <div class="blt2__top face"> </div>
      <div class="blt2__bottom face"> </div>
    </div>
    <div class="blb">
      <div class="blb__front face"> </div>
      <div class="blb__back face"> </div>
      <div class="blb__right face"> </div>
      <div class="blb__left face"> </div>
      <div class="blb__top face"> </div>
      <div class="blb__bottom face"> </div>
    </div>
    <div class="blb2">
      <div class="blb2__front face"> </div>
      <div class="blb2__back face"> </div>
      <div class="blb2__right face"> </div>
      <div class="blb2__left face"> </div>
      <div class="blb2__top face"> </div>
      <div class="blb2__bottom face"> </div>
    </div>
    <div class="puerta-c">
      <div class="puerta">
        <div class="puerta__front face"> </div>
        <div class="puerta__back face"> </div>
        <div class="puerta__right face"> </div>
        <div class="puerta__left face"> </div>
        <div class="puerta__top face"> </div>
        <div class="puerta__bottom face"> </div>
      </div>
      <div class="puerta-l">
        <div class="puerta-l__front face"> </div>
        <div class="puerta-l__back face"> </div>
        <div class="puerta-l__right face"> </div>
        <div class="puerta-l__left face"> </div>
        <div class="puerta-l__top face"> </div>
        <div class="puerta-l__bottom face"> </div>
      </div>
      <div class="puerta-r">
        <div class="puerta-r__front face"> </div>
        <div class="puerta-r__back face"> </div>
        <div class="puerta-r__right face"> </div>
        <div class="puerta-r__left face"> </div>
        <div class="puerta-r__top face"> </div>
        <div class="puerta-r__bottom face"> </div>
      </div>
      <div class="puerta-t">
        <div class="puerta-t__front face"> </div>
        <div class="puerta-t__back face"> </div>
        <div class="puerta-t__right face"> </div>
        <div class="puerta-t__left face"> </div>
        <div class="puerta-t__top face"> </div>
        <div class="puerta-t__bottom face"> </div>
      </div>
    </div>
    <div class="cuadro-l">
      <div class="cuadro-l__front face"> </div>
      <div class="cuadro-l__back face"> </div>
      <div class="cuadro-l__right face"> </div>
      <div class="cuadro-l__left face"> </div>
      <div class="cuadro-l__top face"> </div>
      <div class="cuadro-l__bottom face"> </div>
    </div>
    <div class="cuadro-r">
      <div class="cuadro-r__front face"> </div>
      <div class="cuadro-r__back face"> </div>
      <div class="cuadro-r__right face"> </div>
      <div class="cuadro-r__left face"> </div>
      <div class="cuadro-r__top face"> </div>
      <div class="cuadro-r__bottom face"> </div>
    </div>
    <div class="librero">
      <div class="librero__front face"> </div>
      <div class="librero__back face"> </div>
      <div class="librero__right face"> </div>
      <div class="librero__left face"> </div>
      <div class="librero__top face"> </div>
      <div class="librero__bottom face">    </div>
    </div>
    <div class="libros">
      <div class="libro">
        <div class="libro__front face"> </div>
        <div class="libro__back face"> </div>
        <div class="libro__right face"> </div>
        <div class="libro__left face"> </div>
        <div class="libro__top face"> </div>
        <div class="libro__bottom face"> </div>
      </div>
      <div class="libro">
        <div class="libro__front face"> </div>
        <div class="libro__back face"> </div>
        <div class="libro__right face"> </div>
        <div class="libro__left face"> </div>
        <div class="libro__top face"> </div>
        <div class="libro__bottom face"> </div>
      </div>
      <div class="libro">
        <div class="libro__front face"> </div>
        <div class="libro__back face"> </div>
        <div class="libro__right face"> </div>
        <div class="libro__left face"> </div>
        <div class="libro__top face"> </div>
        <div class="libro__bottom face"> </div>
      </div>
      <div class="libro">
        <div class="libro__front face"> </div>
        <div class="libro__back face"> </div>
        <div class="libro__right face"> </div>
        <div class="libro__left face"> </div>
        <div class="libro__top face"> </div>
        <div class="libro__bottom face"> </div>
      </div>
      <div class="libro">
        <div class="libro__front face"> </div>
        <div class="libro__back face"> </div>
        <div class="libro__right face"> </div>
        <div class="libro__left face"> </div>
        <div class="libro__top face"> </div>
        <div class="libro__bottom face"> </div>
      </div>
      <div class="libro">
        <div class="libro__front face"> </div>
        <div class="libro__back face"> </div>
        <div class="libro__right face"> </div>
        <div class="libro__left face"> </div>
        <div class="libro__top face"> </div>
        <div class="libro__bottom face"> </div>
      </div>
    </div>
    <div class="fotos">
      <div class="foto">
        <div class="foto__front face"> </div>
        <div class="foto__back face"> </div>
        <div class="foto__right face"> </div>
        <div class="foto__left face"> </div>
        <div class="foto__top face"> </div>
        <div class="foto__bottom face"> </div>
      </div>
      <div class="foto">
        <div class="foto__front face"> </div>
        <div class="foto__back face"> </div>
        <div class="foto__right face"> </div>
        <div class="foto__left face"> </div>
        <div class="foto__top face"> </div>
        <div class="foto__bottom face"> </div>
      </div>
    </div>
    <div class="cajas">
      <div class="caja">
        <div class="caja__front face"> </div>
        <div class="caja__back face"> </div>
        <div class="caja__right face"> </div>
        <div class="caja__left face"> </div>
        <div class="caja__top face"> </div>
        <div class="caja__bottom face"> </div>
      </div>
      <div class="caja">
        <div class="caja__front face"> </div>
        <div class="caja__back face"> </div>
        <div class="caja__right face"> </div>
        <div class="caja__left face"> </div>
        <div class="caja__top face"> </div>
        <div class="caja__bottom face"> </div>
      </div>
      <div class="caja">
        <div class="caja__front face"> </div>
        <div class="caja__back face"> </div>
        <div class="caja__right face"> </div>
        <div class="caja__left face"> </div>
        <div class="caja__top face"> </div>
        <div class="caja__bottom face"> </div>
      </div>
    </div>
    <div class="tv">
      <div class="tv__front face"> </div>
      <div class="tv__back face"> </div>
      <div class="tv__right face"> </div>
      <div class="tv__left face"> </div>
      <div class="tv__top face"> </div>
      <div class="tv__bottom face"> </div>
    </div>
    <div class="repisa-t">
      <div class="repisa-t__front face"> </div>
      <div class="repisa-t__back face"> </div>
      <div class="repisa-t__right face"> </div>
      <div class="repisa-t__left face"> </div>
      <div class="repisa-t__top face"> </div>
      <div class="repisa-t__bottom face"> </div>
    </div>
    <div class="repisa-b">
      <div class="repisa-b__front face"> </div>
      <div class="repisa-b__back face"> </div>
      <div class="repisa-b__right face"> </div>
      <div class="repisa-b__left face"> </div>
      <div class="repisa-b__top face"> </div>
      <div class="repisa-b__bottom face"> </div>
    </div>
    <div class="bocina-l">
      <div class="bocina-l__front face"> </div>
      <div class="bocina-l__back face"> </div>
      <div class="bocina-l__right face"> </div>
      <div class="bocina-l__left face"> </div>
      <div class="bocina-l__top face"> </div>
      <div class="bocina-l__bottom face"> </div>
    </div>
    <div class="bocina-r">
      <div class="bocina-r__front face"> </div>
      <div class="bocina-r__back face"> </div>
      <div class="bocina-r__right face"> </div>
      <div class="bocina-r__left face"> </div>
      <div class="bocina-r__top face"> </div>
      <div class="bocina-r__bottom face"> </div>
    </div>
    <div class="muro">
      <div class="muro__front face"> </div>
      <div class="muro__back face"> </div>
      <div class="muro__right face"> </div>
      <div class="muro__left face"> </div>
      <div class="muro__top face"> </div>
      <div class="muro__bottom face"> </div>
    </div>
    <div class="sillon-c">
      <div class="sillon-b">
        <div class="sillon-b__front face"> </div>
        <div class="sillon-b__back face"> </div>
        <div class="sillon-b__right face"> </div>
        <div class="sillon-b__left face"> </div>
        <div class="sillon-b__top face"> </div>
        <div class="sillon-b__bottom face"> </div>
      </div>
      <div class="sillon-t">
        <div class="sillon-t__front face"> </div>
        <div class="sillon-t__back face"> </div>
        <div class="sillon-t__right face"> </div>
        <div class="sillon-t__left face"> </div>
        <div class="sillon-t__top face"> </div>
        <div class="sillon-t__bottom face"> </div>
      </div>
      <div class="sillon-l">
        <div class="sillon-l__front face"> </div>
        <div class="sillon-l__back face"> </div>
        <div class="sillon-l__right face"> </div>
        <div class="sillon-l__left face"> </div>
        <div class="sillon-l__top face"> </div>
        <div class="sillon-l__bottom face"> </div>
      </div>
      <div class="sillon-r">
        <div class="sillon-r__front face"> </div>
        <div class="sillon-r__back face"> </div>
        <div class="sillon-r__right face"> </div>
        <div class="sillon-r__left face"> </div>
        <div class="sillon-r__top face"> </div>
        <div class="sillon-r__bottom face"> </div>
      </div>
    </div>
    <div class="mesa-c">
      <div class="mesa">
        <div class="mesa__front face"> </div>
        <div class="mesa__back face"> </div>
        <div class="mesa__right face"> </div>
        <div class="mesa__left face"> </div>
        <div class="mesa__top face"> </div>
        <div class="mesa__bottom face"> </div>
      </div>
      <div class="mesa-p">
        <div class="mesa-p__front face"> </div>
        <div class="mesa-p__back face"> </div>
        <div class="mesa-p__right face"> </div>
        <div class="mesa-p__left face"> </div>
        <div class="mesa-p__top face"> </div>
        <div class="mesa-p__bottom face"> </div>
      </div>
      <div class="mesa-p">
        <div class="mesa-p__front face"> </div>
        <div class="mesa-p__back face"> </div>
        <div class="mesa-p__right face"> </div>
        <div class="mesa-p__left face"> </div>
        <div class="mesa-p__top face"> </div>
        <div class="mesa-p__bottom face"> </div>
      </div>
      <div class="mesa-p">
        <div class="mesa-p__front face"> </div>
        <div class="mesa-p__back face"> </div>
        <div class="mesa-p__right face"> </div>
        <div class="mesa-p__left face"> </div>
        <div class="mesa-p__top face"> </div>
        <div class="mesa-p__bottom face"> </div>
      </div>
      <div class="mesa-p">
        <div class="mesa-p__front face"> </div>
        <div class="mesa-p__back face"> </div>
        <div class="mesa-p__right face"> </div>
        <div class="mesa-p__left face"> </div>
        <div class="mesa-p__top face"> </div>
        <div class="mesa-p__bottom face"> </div>
      </div>
      <div class="mesa-shadow"></div>
    </div>
    <div class="tablet">
      <div class="tablet__front face"> </div>
      <div class="tablet__back face"> </div>
      <div class="tablet__right face"> </div>
      <div class="tablet__left face"> </div>
      <div class="tablet__top face"> </div>
      <div class="tablet__bottom face">    </div>
    </div  </div        
            </div>
        </foreignObject>
    </svg>
