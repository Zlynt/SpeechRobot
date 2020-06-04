# SpeechRobot
 Framework that facilitates the use of Text to Speech or Speech to Text
 
 ## How to use
 
 1) Include the script in your page
 <script src="/SpeechRobotDemo/SpeechRobot.js"></script>
 
 2) Create a new variable
 let speechRobot = new SpeechRobot();
 
3) If you want to:

-> Make the browser speak

speechRobot.speak('en-US', 'Hello World!');

-> Make the browser understand the speech

//Start the speech to text

speechRobot.listen('en-US', (recognized_sentence) => {

 console.log("I heard: "+recognized_sentence);
 
});

//Stop the speech to text after 5 seconds

setTimeout(() => {

 speechRobot.stopListening();
 
}, 5000);
