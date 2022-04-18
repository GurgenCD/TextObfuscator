# TextObfuscator
A simple obfuscating script that animates desired text

# How it works
1. The text that is entered in the **text** variable is split into individual letters, stored in an array
2. Each letter has a separate declared array, which acts as a place to store characters that will be used to replace that specific letter down the line
3. a for() function is run for each letter in the array, which using eval() function finds its' individual array. It then randomly chooses the element in the letter's array. 2 random characters are then chosen to replace the original characters.
4. a parent for() function runs the 3rd step 100 times, and then stores it in an array.
