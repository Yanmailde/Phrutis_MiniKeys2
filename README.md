# MiniKeys2
![Serie1 coins](https://user-images.githubusercontent.com/82582647/185912181-afcef4e1-2c4b-4be1-be52-1e5d5a14511c.png)

This is the fastest program to find old Serie1 minikeys in the world.

## Quick start

For RTX 2070, 2080</br>
Run: ```MiniKeys2-20xx.exe -bits 24 -a addresses.txt -d 0```</br>

For RTX 3060, 3070, 3080</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 0```</br>

For RTX 3090, A100, A5000, A6000</br>
Run: ```MiniKeys2-30xx.exe -bits 25 -a addresses.txt -d 0```<hr>

### Extra options

-d ? - Card number</br>
-a ? - Name of BTC address database 1.., 3.., bc... on a new line</br>
-id ? - Telegram bot chat number</br>
-bot ? - bot token (create your bot)</br>
-test (Checking the operation of FOUND and sending a message to you in telegram)</br>

1Cdr4SMTmm4ViY5nZdrygJ2xAJ1qVi41oM</br>
1NiNKjngcQBnCyw9VZZMa6cW2ngku6KM7G</br>
3E8VWzznxTpesgXoAT24wxsD4fUgHJeSNd</br>
bc1qackhakrjwspscnmsdl93ayrxt52plug8ffjjep</br>

To test, add one of these address (or all) to the database</br>
Run a quick test (18 bits):</br>
```MiniKeys2-20xx.exe -bits 18 -a addresses.txt -id 123456789 -bot 1122334455:ABG5X3XU0upZQ8ELkR-EYR9C4OfBEVHBFKQ -d 0 -test```</br></br>
![test-bot](https://user-images.githubusercontent.com/82582647/185806061-4c7d3471-98d6-4a61-ae9c-83e6c96936c8.png)

| Minikeys2 GPU Speed |
|---------------------------|

| GPU card   | -bits    | Speed    |
|------------|----------|----------|
| A100       | 26       | 12 Gkeys |
| A6000      | 25       | 11 Gkeys |
| 3090       | 25       | 10 Gkeys |
| 3080 Ti    | 24       | 10 Gkeys |
| 3080       | 24       | 8.5 Gkeys |
| 3070 Ti    | 24       | ? Gkeys  |
| 3070       | 24       | ? Gkeys  |
| 3060       | 24       | ? Gkeys  |
| 2080 S     | 24       | ? Gkeys  |
| 2070       | 24       | 2 Gkeys  |

## Special version 1.1 
For rigs with a lot of cards and little RAM (8 GB)</br>
One GPU consumes only 480 MB of RAM</br>
The program only supports old addresses 1..</br>
Everything else is the same as in the standard program v1.0</br>

For RTX 2070, 2080</br>
Run: ```M20xx.exe -bits 23 -a addresses.txt -d 0```</br>

For RTX 3060, 3070, 3080</br>
Run: ```M30xx.exe -bits 23 -a addresses.txt -d 0```</br>

For RTX 3090, A100, A5000, A6000</br>
Run: ```M30xx.exe -bits 25 -a addresses.txt -d 0```</br></br>
Run a quick test:</br>
```M30xx.exe -bits 18 -a addresses.txt -d 0 -test```</br></br>
![v1.1](https://user-images.githubusercontent.com/82582647/185807241-0a4b8a62-fb24-47f8-bf31-4d97ad8789e9.png)

| M20xx, M30xx GPU Speed |
|---------------------------|

| GPU card   | -bits    | Speed    |
|------------|----------|----------|
| A100       | 26       | ? Gkeys |
| A6000      | 25       | ? Gkeys |
| 3090       | 25       | ? Gkeys |
| 3080 Ti    | 23       | ? Gkeys  |
| 3080       | 23       | ? Gkeys  |
| 3070 Ti    | 23       | ? Gkeys  |
| 3070       | 23       | ? Gkeys  |
| 3060       | 23       | ? Gkeys  |
| 2080 S     | 23       | ? Gkeys  |
| 2070       | 23       | 2.2 Gkeys  |

## :wrench: How it works?
[**Read more about TURBO+ and Random modes**](https://github.com/phrutis/MiniKeys2/blob/main/Others/work.md)

### :memo: Frequently Asked Questions<hr>
Where to download the program, how to run it?</br>

[**HERE**](https://github.com/phrutis/MiniKeys2/releases/tag/1.0)<hr>

Where can I download the database of OLD BTC addresses 1... ?</br>

[**HERE**](https://github.com/phrutis/MiniKeys2/releases/tag/1.0)<hr>

Where to download 4907 addresses of coins series1?</br>

[**HERE**](https://github.com/phrutis/MiniKeys2/blob/main/Others/serie1.txt)<hr>

How many physical coins were issued and which ones?</br>

61,560 coins. List of all addresses from coins and other information [**HERE**](https://raw.githubusercontent.com/phrutis/MiniKeys2/main/Others/Fullist.txt)<hr> 

Does the program require an internet connection?</br>
If you use a telegram bot - Yes</br>
If you just search, you don't need internet.<hr>

I launched the program hung (froze) what should I do?</br>

The program needs time to create the table.</br>
Wait for start:</br>
For 23 bits = 20 minutes</br>
For 24 bits = 25 minutes</br>
For 25 bits = 35 minutes</br>
For 26 bits = 45 minutes<hr>

If I find the private key can I take all the coins for myself?</br>

No, you will find the encrypted key.</br>
Only the organizers  can decrypt this key and pay you a 50%.<hr>

I have a RTX 3060 TI card, and I have a low speed, how can speed up?</br>

In the new drivers for 30xx Ti, 20xx Ti, a limiter is installed that slows down the speed by half.</br>
You need to download the old driver from six months ago. 496.13</br>
Delete the new driver, install the old driver, the speed will increase x2</br>
After searching, you can install new drivers.<hr>

I have many GPUs. How to start?

Run each GPU separately. Add your card id -d ?</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 0```</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 1```</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 2```</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 3```</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 4```</br></br>
To run one gpu in ```MiniKeys2``` you need 4-6 GB of RAM!</br>
If you are low on RAM, use the ```M30xx``` program.</br>
It only needs 500 MB of RAM to run.<hr>

Why didn't you do a Serie2 30 character minikey search?</br>

These are new coins (2013)</br>
Very large search range.</br>
Many coins are nominal, the amounts are small.</br>
They can also be found in random.<hr>

How to find out that the program has found the key?</br>

A message about the find will appear in the program window.</br>
The program will also write the address and key to the text file FOUND.txt</br>
If a telegram bot is connected, it will send you a message.<hr>

How to create a bot and get id ?</br>

Find information on the Internet.<hr>

Why did the program open the browser?</br>

Sending API telegram bot requests goes only through the browser.<hr>

What is the chance to find?</br>

Just like winning the lottery.<hr>

Is this theft?

This is a very controversial issue!</br>
Almost all coins are lost.</br>
Coins (Serie1) are 12 years old, with a high rate of bitcoin, they were not used.</br>
Or do you think that the owner of the coin is waiting for the rate to fall at all?</br>
If you find a gold coin on the beach (in a landfill)?</br>
Is this theft or a find?</br>
After all, the found coin has (was) an owner, you didn’t physically steal it.</br>
It's just that the lost coin has a new owner.</br>
As the unspoken rule of bitcoin says:</br>
Whoever has the private key is the owner.</br>
Try to find it first :-)<hr>

If I find a large amount (more than 1 btc), what are the guarantees that I will receive my 50%?

At the moment there is no way to give you a guarantee.</br>
Suggest your way.</br>
The payment is based on trust.</br>
If the amount is large and there is no trust, you can fly to Belarus Minsk and meet in person.</br>
Import and send coins will be in your presence at the hotel.<hr>

What is rated speed?</br>

The RTX 3090 can process max 180,000,000 minikeys (private keys) per second.</br>
Since invalid private keys after validation ? == 00 are skipped, which increases the speed.</br>
Example</br>
10,000,000,000 (mini-keys) private keys were processed, of which only</br>
180,000,000 turned out to be valid and went through the full cycle of the private key -> address algorithm.</br>
The remaining 9,820,000,000 were skipped in the first stage.</br>
For clarity, let's take a minikey</br>
SkK5VPtmTm3mQKYaJQFRZP his private key f30c1ddd12ea91bd35d5d1b83eac611717d99da826f207c3c3d4839e271648cb</br>
To check the validity of the minikey, you need to add "?"</br>
SkK5VPtmTm3mQKYaJQFRZP? -> sha256 = 00442b142a40eefcd894b0bb6f19c58284f2e7248cee7e4910cd37afbfc7879a</br>
If the output private key starts with 00...., then</br>
The minikey (without the ?) is valid and needs to be processed.</br>
If you change one letter of the minikey and add "?" you don't get a private key that starts with 00....</br>
According to statistics, only 1 key out of 50-60 will be valid.<hr>

When FOUND is triggered, the last position of the minikey is visible.</br>
I will pass in Fialka M-125 7 characters and will not share with you.</br>

The toolbar displays a part of the random key that is not included in the search.</br>
This was done for the visual process of the program.<hr>

I didn't find the answer to my question<hr>

Write your question [**HERE**](https://github.com/phrutis/MiniKeys2/issues)<hr>

### Disclaimer
PROGRAM AND INFORMATION ARE FOR EDUCATIONAL PURPOSES ONLY. USE IT AT YOUR OWN RISK. THE DEVELOPER WILL NOT BE RESPONSIBLE FOR ANY LOSS, DAMAGE OR CLAIM ARISING FROM USING THIS PROGRAM
