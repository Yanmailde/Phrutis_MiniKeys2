## :wrench: How it works

RTX 3090 Speed = 180,000,000/s

By checking the [validity of keys](https://en.bitcoin.it/wiki/Mini_private_key_format), speed increased to 10,000,000,000/s</br>

Number of minikeys Serie1 = 4907</br> 
Denomination of coins 1, 5, 10, 25, 500, 1000 BTC</br>

In 2011-2012 bitcoin was worth cents.</br>
The coins did not provide crypto value.</br>
Beautiful physical coins were used as souvenirs, given as gifts, lost, thrown away.</br>
Many people simply did not know that there was a mini-key under the holagram.</br>
Suppose the person knew about the key</br>
2011 1 btc = $0.08</br>
Where can I spend $0.08?</br>
2012 year 1 btc = $1</br>
In 2013 you can buy pizza :)</br>
Then the rate began to rise.</br>

According to the [**analysis**](https://casascius.uberbills.com) of discoveries, you can see that coins began to be opened until 2017.</br>
When in 2021 the bitcoin rate peaked at 1 btc = $60,000, there were no coins discovered?!</br>
This suggests one thing, all possible (available) coins have already been discovered previously.</br>

After 2017, there were only 6 coins discovered!</br>
31.12.2020 and 31.12.2021 [**6 coins were opened**](https://casascius.uberbills.com/?status=opened), of which 3 coins are Serie1 and 3 are new coins (Serie2 30 symbols)</br>
Based on these assumptions, we can conclude that 95% (out of 4907) Serie1 coins are losses.</br>
5% are possibly used as collectibles.</br>

There are 22 minikey combinations in total</br>
S+21 base58 characters.</br>
Total 21 characters:</br>
10,764,351,351,569,111,513,009,094,806,216,900,608 combinations.</br>

When analyzing public minikeys ([see gallery](https://github.com/phrutis/MiniKeys2/issues/1)), as well as generating in the original minikey generator
was defined:

In minikeys (as well as in words) there are no 3 identical letters in a row.</br>
A valid random almost does not give 3 (4, 5) identical letters in a row.

Based on this statement, the TURBO+ algorithm was created, which eliminates 3 identical letters in a row.

Clearly not a valid key:</br>
SSSa58hDA3kpvFQuubBc8Wn</br>
Anything after SSS is not valid.</br>
We exclude the range after.</br>
SSS~~1111111111111111111~~ -> SSS~~zzzzzzzzzzzzzzzzzz~~</br>

Total combinations:</br>
10,764,351,351,569,111,513,009,094,806,216,900,608

The TURBO+ algorithm is subtracted from the total:</br>
SSS.....</br>
-3,199,866,632,452,173,458,088,315,935,260,672</br>
SSs.....</br>
-3,199,866,632,452,173,458,088,315,935,260,672</br>
SsS.....</br>
-3,199,866,632,452,173,458,088,315,935,260,672</br>
Sss.....</br>
-3,199,866,632,452,173,458,088,315,935,260,672</br>

SAAA...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
SAAa...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
SAaa...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
SaaA...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
SaAa...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
SAaA...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
Saaa...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>

Sxaaa.., ScvxXx..., SktbEeE... SDai5WmgdEq5bbB... etc.</br>
In total, more than 220+ variations of replacement combinations along the entire length.

Outcome.</br>
Tatal 21 symbols (without turbo):</br>
10,764,351,351,569,111,513,009,094,806,216,900,608

Total 21 symbols (TURBO+)</br>
751,281,569,183,509,134,909,325,127,825*

*Approximately (did not count)</br>
Less total - more chances.</br>
There are a lot of combinations, you just need to hope for luck.

The TURBO+ algorithm not only eliminates 3 identical letters, but also replaces "+" with the next letter.</br>
Random example:</br>
SGayRrR... -> SGayRrT...</br>
SavdEee... -> SavdEef...</br></br>

### FULL Random

S...... -> sha256 = private key.</br>
Each private key output from sha256 is unique. It is 100% random and valid.</br>

By this, you can find any address 1 ... from the database !!!</br>
Even if the address was generated randomly in bitcoin core.</br> 
It's just that the private key corresponds to the minikey's private key.</br>
This is a feature of the bitcoin algorithm.</br>

The main advantage of mode 2 is speed x2</br>
The program works in two modes Uncompressed and Compressed</br>
RTX 3090 Rated Speed = 180,000,000 minikeys per second</br>
That's 180,000,000 random private keys per second.</br>
Since we are searching in two modes at once, this is 180,000,000x2=360,000,000 addresses per second.</br>
There is also a great chance to find an address collision.</br>
Example</br>
The private key 5cdd2f650aa61749a0c0d101bc80c454877ead2b6671654cc9bc99633120704e corresponds to the uncompressed address 1Deho8FnoB6veE5Zq7KcEDmUHoaSm1mVyA</br>
The private key f418546ef63340cd426083f3d0ddfa48421db5717fa8c97201cc3d4e92507b98 can match compressed key 1Deho8FnoB6veE5Zq7KcEDmUHoaSm1mVyA</br>

Additionally:</br>
Possible collision hex160 (rimpd160)</br>
Since the range of hashes160 is 160 bits, and private keys are 256 bits.</br>

One address from the database (hash160) =</br> 
79,228,162,514,264,337,593,543,950,336 private keys in 256 bits in compressed mode.</br>
+79.228.162.514.264.337.593.543.950.336 in uncompressed mode.</br>

We get a total of 158,456,325,028,528,675,187,087,900,672 private keys that correspond to one address in 256 bits.</br>
There are more than 17,000,000 addresses in the database.</br>

**This is all in theory, in practice these are very large ranges, you only need to hope for luck.**
