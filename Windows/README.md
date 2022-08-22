## Windows v1.0

For RTX 2070, 2080</br>
Run: ```MiniKeys2-20xx.exe -bits 24 -a addresses.txt -d 0```

For RTX 3060, 3070, 3080</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 0```

For RTX 3090, A100, A5000, A6000</br>
Run: ```MiniKeys2-30xx.exe -bits 25 -a addresses.txt -d 0```

For RTX A100, A5000, A6000</br>
Run: ```MiniKeys2-30xx.exe -bits 26 -a addresses.txt -d 0```
<hr>

### Windows v1.1 For RIG If 2-8 cards and little RAM (8GB)

One GPU consumes only 480 MB of RAM</br>
**The program only supports old addresses 1...**

For RTX 2070, 2080</br>
Run: ```M20xx.exe -bits 23 -a addresses.txt -d 0```

For RTX 3060, 3070, 3080</br>
Run: ```M30xx.exe -bits 23 -a addresses.txt -d 0```

For RTX 3090</br>
Run: ```M30xx.exe -bits 25 -a addresses.txt -d 0```

For RTX A100, A5000, A6000</br>
Run: ```M30xx.exe -bits 26 -a addresses.txt -d 0```

-d ? - Card number</br>
-a ? - Name of BTC address database 1.., 3.., bc... on a new line</br>
-id ? - Telegram BOT chat id</br>
-bot ? - bot token (your bot)</br>
-test (Checking the operation of FOUND and sending a message to you in telegram)</br>

#### TEST

Addresses for the test:</br>
1Cdr4SMTmm4ViY5nZdrygJ2xAJ1qVi41oM</br>
1NiNKjngcQBnCyw9VZZMa6cW2ngku6KM7G</br>
3E8VWzznxTpesgXoAT24wxsD4fUgHJeSNd</br>
bc1qackhakrjwspscnmsdl93ayrxt52plug8ffjjep

To test, add one of these address (or all) to the database (addresses.txt)</br>
Quick test FOUND:</br>
Run: ```MiniKeys2-30xx.exe -bits 18 -a addresses.txt -d 0 -test```

Run a quick test Telegram BOT:</br>
```MiniKeys2-30xx.exe -bits 18 -a addresses.txt -id 123456789 -bot 1122334455:ABG5X3XU0upZQ8ELkR-EYR9C4OfBEVHBFKQ -d 0 -test```<hr>
