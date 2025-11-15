<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>English App – Beginner Lesson</title>

<style>
    body {
        font-family: Arial, sans-serif;
        background: #f5f6fa;
        margin: 0;
        padding: 0;
    }

    header {
        background: #4A90E2;
        color: white;
        padding: 20px;
        text-align: center;
        font-size: 24px;
        font-weight: bold;
    }

    .section {
        padding: 20px;
    }

    h2 {
        color: #333;
        margin-bottom: 10px;
        border-left: 4px solid #4A90E2;
        padding-left: 10px;
    }

    .card {
        background: white;
        border-radius: 12px;
        padding: 15px;
        box-shadow: 0 3px 8px rgba(0,0,0,0.1);
        margin-bottom: 12px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .audioBtn {
        background: #4A90E2;
        color: white;
        border: none;
        padding: 10px 14px;
        border-radius: 8px;
        font-size: 18px;
        cursor: pointer;
    }

    .quiz-option {
        background: white;
        padding: 12px;
        border-radius: 8px;
        margin-top: 8px;
        cursor: pointer;
        border: 2px solid transparent;
    }

    .quiz-option:hover {
        background: #e8f1ff;
    }

    .correct {
        border-color: #2ecc71 !important;
        background: #eaffea !important;
    }

    .wrong {
        border-color: #e74c3c !important;
        background: #ffeaea !important;
    }
</style>

<script>
    function playAudio(src) {
        new Audio(src).play();
    }

    function checkAnswer(element, correct) {
        if (correct) {
            element.classList.add("correct");
        } else {
            element.classList.add("wrong");
        }
    }
</script>

</head>
<body>

<header>English Lesson – Greetings</header>

<div class="section">
    <h2>Vocabulary</h2>

    <div class="card">
        <span>Hello – Olá</span>
        <button class="audioBtn" onclick="playAudio('audio/hello.mp3')">🔊</button>
    </div>

    <div class="card">
        <span>Hi – Oi</span>
        <button class="audioBtn" onclick="playAudio('audio/hi.mp3')">🔊</button>
    </div>

    <div class="card">
        <span>Good morning – Bom dia</span>
        <button class="audioBtn" onclick="playAudio('audio/goodmorning.mp3')">🔊</button>
    </div>

    <div class="card">
        <span>Good afternoon – Boa tarde</span>
        <button class="audioBtn" onclick="playAudio('audio/goodafternoon.mp3')">🔊</button>
    </div>

    <div class="card">
        <span>Good evening – Boa noite</span>
        <button class="audioBtn" onclick="playAudio('audio/goodevening.mp3')">🔊</button>
    </div>

    <div class="card">
        <span>Goodbye – Tchau</span>
        <button class="audioBtn" onclick="playAudio('audio/goodbye.mp3')">🔊</button>
    </div>

</div>


<div class="section">
    <h2>Useful Phrases</h2>

    <div class="card">
        <span>Hello, how are you? – Olá, como vai?</span>
        <button class="audioBtn" onclick="playAudio('audio/howareyou.mp3')">🔊</button>
    </div>

    <div class="card">
        <span>I'm fine, thank you – Estou bem, obrigado</span>
        <button class="audioBtn" onclick="playAudio('audio/imfine.mp3')">🔊</button>
    </div>

    <div class="card">
        <span>What's your name? – Qual seu nome?</span>
        <button class="audioBtn" onclick="playAudio('audio/whatsyourname.mp3')">🔊</button>
    </div>
</div>


<div class="section">
    <h2>Mini Quiz</h2>

    <p><strong>1. “How are you?” significa:</strong></p>

    <div class="quiz-option" onclick="checkAnswer(this, false)">A) Quem é você</div>
    <div class="quiz-option" onclick="checkAnswer(this, true)">B) Como você está</div>
    <div class="quiz-option" onclick="checkAnswer(this, false)">C) Onde você mora</div>

<br>

    <p><strong>2. “Thank you” significa:</strong></p>

    <div class="quiz-option" onclick="checkAnswer(this, false)">A) Olá</div>
    <div class="quiz-option" onclick="checkAnswer(this, true)">B) Obrigado</div>
    <div class="quiz-option" onclick="checkAnswer(this, false)">C) Tchau</div>
</div>

</body>
</html>
