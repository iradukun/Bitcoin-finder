# Bitcoin-Finder
Generate random bitcoin wallets & private keys (seeds) and then check if they match any wallet that has a positive balance, and then take all the btc from it.

# CHANGELOG
<details>
   <summary>2024-01-11</summary>
   
   - Now calling garbage collector to potentially stop from memory leaking
   - Releasing references to objects to allow the gc reclaim the memory
   - Loading riches.txt contents to a map() object to increase the scripts overall performance
</details>

<details>
   <summary>2024-01-01</summary>
  
   - Added a message to console when program starts, to calm down people who think the program isn't working because the console is blank.
</details>

<details>
   <summary>2023-12-09</summary>
  
   - Fixed big memory leak issue and removed extra scripts that were necessary before, that are unnecesary now.
</details>

<details>
   <summary>2023-09-26</summary>
  
   - Linux support: linux users will go to the "linux" directory to run the program.
</details>

# REQUIREMENTS
1. Install Node.js
2. npm i
3. Lots of time on your hands.. there's a lot and I mean A LOT of possible addresses and keys, you will be extremely lucky to find any that will match your list.

# HOW TO RUN
Just start run.bat (or run.sh if you're on linux).

# SPEED / PERFORMANCE
Results from a somewhat decent computer:
- 1.56 million checks every 1 minute
- 7.2 billion checks in 1 day
- 54 billion checks in a week
- 216 billion checks in a month
- 2.8 trillion checks in a year

But please keep in mind that this is still really not much compared to all possible combinations that should be checked.

# VIDEO

[![YT VID](http://img.youtube.com/vi/JaKDEWXOKn0/0.jpg)](http://www.youtube.com/watch?v=JaKDEWXOKn0 "Bitcoin - Find Private Keys (Seeds) For Lost and Rich Wallets | NEW 2021")

# TEST IT
Go to the test folder and hit run. It will show you what would happen if a wallet from your list was found.

# WHY DO THIS?
There are a lot of wallets with high balances that are lost forever, which means nobody can access them and the money is basically there just to be picked up by anyone. This program can possibly find these lost wallets and their matching private keys and take the btc out of them.


