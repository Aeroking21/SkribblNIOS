# SkribblNIOS
An online multiplayer drawing game using an FPGA as a drawing tool 

Our objective was to design an IoT system connected via an AWS server and perform local processing on accelerometer data captured by an FPGA. We decided to implement an online multiplayer game inspired by the popular board game Pictionary.  

## How to Play? 
1. The player will be loaded into the main menu where they choose their username, avatar and either input their private server details or leave it blank so they connect to the main server. 
2. There will be an FPGA indicator showing whether the board is connected. If so, the game will load in ‘FPGA mode’, otherwise it will load in ‘mouse mode’ (Mac user support). 
3. When connected, the players will be loaded into a lobby screen. 
4. Initially, the first player to join will be the drawer. After each round a new drawer will be selected randomly by the server. 
5. The drawer is shown a choice of 3 words, they’ll choose 1 to draw using either the FPGA or mouse depending on which mode they’ve chosen. 
6. A timer will begin, and the remaining players will attempt to guess the word using the chat before the round ends. The time display is represented by an array of LEDs that turn on incrementally as time passes. 
7. Players will be rewarded with points if they guess the word correctly based on the length of the word and how fast they guessed it. Their score is displayed on the 8-segment display of the FPGA. 
8. At the end of the game the player with the most points is crowned champion of Skribblnios! 

