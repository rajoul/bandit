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
