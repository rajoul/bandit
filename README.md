# bandit1
```
cat readme   >>> bandit1: boJ9jbbUNNfktd78OOpsqOltutMc3MY1
```
# bandit2
```
>ls -al
>cat ./-   >>> bandit2: CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
```
# bandit3
```
>ls 
>cat "spaces in this filename" or > cat spaces\ in\ this\ filename >>> bandit3: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
```
# bandit4
```
>ls 
>cd inhere
>cat ./.hidden >>> bandit4: pIwrPrtPN36QITSp3EQaw936yaFoFgAB
```
# bandit5
```
>ls 
>cd inhere
>file ./*   (open ASCII text file)
>cat ./-file07 >>> bandit5: koReBOKuIDDepwhWk7jZC0RTdopnAYKh
```
# bandit6
```
>ls 
>cd inhere
>find -type f -readable -size 1033c ! -executable
>cat maybehere07/.file2 >>> bandit6: DXjZPULLxYr17uwoI01bNLQbtFemEgo7
```
# bandit7
```
>ls 
>find / -type f -user bandit7 -group bandit6 -size 33c
>cat /var/lib/dpkg/info/bandit7.password >>> bandit7: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
```
# bandit8
```
>ls 
>cat data.txt | grep ^millionth >>> bandit8: cvX2JJa4CFALtqS87jk27qwqGhBM9plV
```
# bandit9
```
>ls 
>sort data.txt |uniq -u >>> bandit9: UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
```
# bandit10
```
>ls 
> cat data.txt | strings | grep ^==== >>> bandit10: truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
```
# bandit11
```
>ls 
>cat data.txt | base64 --decode >>> bandit11: IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
```
# bandit12
```
>ls 
> cat data.txt | tr '[A-Za-z]' '[N-ZA-Mn-za-m]'>>> bandit12: 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
```
# bandit13
```
>ls 
>mkdir /tmp/rajoul
> cp data.txt  /tmp/rajoul
> cd /tmp/rajoul
>cat data.txt | xxd -r >data1
>mv data1 data1.gz
>gzip -d data1.gz
>bzip2 -d data1
> mv data1.out data1.gz
>gzip -d data1.gz
>mv data1 data1.tar
>tar -xvf data1.tar
>mv data5.bin data5.tar
>tar -xvf data5.tar
> mv data6.bin data6.bz2
>bzip2 -d data6.bz2
>mv data6 data6.tar
>tar -xvf data6.tar
>mv data8.bin data8.gz
>gzip -d data8.gz
>cat data6 >>> bandit13: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
```





