# TextObfuscator
A vanilla JS script that reads the innerText of a div with a "animatedtext" id, generatespatterns in realtime, and cycles between them in order to create a glitch-looking effect

[Check it out](https://imforpeace.github.io/TextObfuscator/)

# How it works
JS script:
1. The text is split into individual letters
2. Each letter is pre-declared as a key in a JSON lettermap object, which acts as a place to store characters that will be used to replace that specific letter down the line
3. The script then takes two letters out of the text div, and sequentially chooses a random character in the lettermap array for that specific letterle
4. a parent for() function runs the 3rd step 100 times, and then stores all results in an array. Note that if the innerText of the animatedtext div is changed, the pattern is regenerated for the new text in realtime.
