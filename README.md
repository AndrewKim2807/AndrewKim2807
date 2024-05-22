<!-- README.md -->
<div id="intro" style="font-family: Arial, sans-serif; text-align: center; font-size: 2em; height: 100px; display: flex; align-items: center; justify-content: center;">
    <span id="hello">Hello</span>
</div>

<script>
const greetings = [
    'Hello', // English
    'Hola', // Spanish
    'Bonjour', // French
    'Hallo', // German
    'Ciao', // Italian
    'こんにちは', // Japanese
    '안녕하세요', // Korean
    '您好', // Chinese
    'Olá', // Portuguese
    'Привет', // Russian
    'مرحبا', // Arabic
    'שלום', // Hebrew
    'नमस्ते', // Hindi
    'สวัสดี', // Thai
    'Kia ora' // Maori
];

let currentGreetingIndex = 0;

function changeGreeting() {
    const helloElement = document.getElementById('hello');
    helloElement.textContent = greetings[currentGreetingIndex];
    currentGreetingIndex = (currentGreetingIndex + 1) % greetings.length;
}

setInterval(changeGreeting, 3000);
</script>

