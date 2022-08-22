# Linux

![A6000](https://user-images.githubusercontent.com/82582647/185991427-e2a4997d-311e-4556-9ecd-31fb5340be77.png)

- ```MiniKeys-20xx``` - v1.0 For RTX 20xx</br>
- ```MiniKeys``` - v1.0 For RTX 30xx

- ```MiniKeys2-20xx``` - v1.1 For RTX 20xx (Min RAM)</br>
- ```MiniKeys2``` - v1.1 For RTX 30xx (Min RAM)
<hr>

# v1.0
For RTX 2060, 2070, 2080</br>
Run: ```chmod +x MiniKeys-20xx```</br>
Run: ```./MiniKeys-20xx -bits 24 -a addresses.txt -d 0```

For RTX 3060, 3070, 3080</br>
Run: ```chmod +x MiniKeys```</br>
Run: ```./MiniKeys -bits 24 -a addresses.txt -d 0```

For RTX 3090</br>
Run: ```chmod +x MiniKeys```</br>
Run: ```./MiniKeys -bits 25 -a addresses.txt -d 0```

For RTX A100, A5000, A6000</br>
Run: ```chmod +x MiniKeys```</br>
Run: ```./MiniKeys -bits 26 -a addresses.txt -d 0```
<hr>

## v1.1 For rig. If 2-8 cards and little RAM (8GB)

For RTX 2060, 2070, 2080</br>
Run: ```chmod +x MiniKeys2-20xx```</br>
Run: ```./MiniKeys2-20xx -bits 23 -a addresses.txt -d 0```

For RTX 3060, 3070, 3080</br>
Run: ```chmod +x MiniKeys2```</br>
Run: ```./MiniKeys2 -bits 23 -a addresses.txt -d 0```

For RTX 3090</br>
Run: ```chmod +x MiniKeys2```
Run: ```./MiniKeys2 -bits 25 -a addresses.txt -d 0```

For RTX A100, A5000, A6000</br>
Run: ```chmod +x MiniKeys2```</br>
Run: ```./MiniKeys2 -bits 26 -a addresses.txt -d 0```
<hr>

-d ? - Card number</br>
-a ? - Name of BTC address database 1.., 3.., bc... on a new line</br>
-test (Checking the operation of FOUND)

1Cdr4SMTmm4ViY5nZdrygJ2xAJ1qVi41oM</br>
1NiNKjngcQBnCyw9VZZMa6cW2ngku6KM7G</br>
3E8VWzznxTpesgXoAT24wxsD4fUgHJeSNd</br>
bc1qackhakrjwspscnmsdl93ayrxt52plug8ffjjep

To test, add one of these address (or all) to the database</br>
Quick test:</br>
Run: ```./MiniKeys -bits 18 -a addresses.txt -d 0 -test```
<hr>
