# Typing-Animation
Typing Animation using css


<h1>HTML</h1>

<code>
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>Page Title</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>
<body>

    <div class="typing">
        <h1>Put your title here..</h1>
    </div>
    
</body>
</html>

</code>



<h1>CSS</h1>

<code>


html, body{
    display: block;
    width: 100%;
    height: 100%;
    background: #000;
    color: #fff;
    padding: 0;
    margin: 0;
}

.typing > *{
    overflow: hidden;
    white-space: nowrap;
    animation: typingAnim 5s steps(50);
}

.typing > *::after{
    content: ". .";
    display: block;
    position: absolute;
    top: 1em;
    left: .35em;
}


@keyframes typingAnim{
    from { width: 0}
    to { width: 100%}
}

@keyframes typingSpeak{
    0% {width: 1em; height: .1em}
    100% { width: 1em; height: .5em}
}
</code>
