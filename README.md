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
# bandit14
```
>ls 
>ssh -i sshkey.private bandit14@localhost
> cat /etc/bandit_pass/bandit14 >>> bandit14: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
```
# bandit15
```
>ls 
> echo '4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e' | nc localhost 30000 >>> bandit15: BfMYroe26WYalil77FoDi9qh59eK5xNr
```
# bandit16
```
>ls 
> echo 'BfMYroe26WYalil77FoDi9qh59eK5xNr'| openssl s_client -connect localhost:30001 >>> bandit16: cluFn7wTiGryunymYOu4RcffSxQluehd
```
# bandit17
```
>ls 
>nmap localhost -p 31000-32000
>echo 'cluFn7wTiGryunymYOu4RcffSxQluehd' |openssl s_client -connect localhost:31790
>mkdir /tmp/rajoul
>cd /tmp/rajoul
>nano private_key.key (then copy paste the RSA priavte key)
>chmod 700 private_key.key
>ssh -i private_key.key bandit17@localhost
>cat /etc/bandit_pass/bandit17 >>> bandit17: xLYVMN9WE5zQ5vHacb0sZEVqbrp7nBTn
```

# bandit18
```
>ls 
> diff passwords.new passwords.new >>> bandit18: kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
```
# bandit20
```
>ls 
> ./bandit20-do cat /etc/bandit_pass/bandit20 >>> bandit20 : GbKksEFF4yrVs6il55v6gwY5aVje5f0j
```
# bandit21
```
>ls 
j'ouvre une autre session puis je lance le serveur en mode ecoute: >nc -l -p 2323
dans l'autre session :>./suconnect 2323
>j'entre le mot de pass dans la première session
>enfin je recois immédiatement le pass de bandit21 >>>> bandit21 : gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr
```
# bandit22
```
>ls 
>cd /etc/cron.d/
> cat cronjob_bandit22
> cat  /usr/bin/cronjob_bandit22.sh
>cat  /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv >>> bandit22 : Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI
```
# bandit23
```
>ls 
>cd /etc/cron.d/
> cat cronjob_bandit23
>cat /usr/bin/cronjob_bandit23.sh
>$(echo I am bandit23 | md5sum | cut -d ' ' -f 1) ==>>>d7387859980fe85c84d68d50eedd8598
> cat /tmp/d7387859980fe85c84d68d50eedd8598 >>> bandit23 : jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n
```
# bandit24
```
>ls 
>cd /etc/cron.d/
> cat cronjob_bandit23
>cat /usr/bin/cronjob_bandit23.sh
donc je cree un fichier dans le /tmp
>mkdir /tmp/rajoul
>cd /tmp/rajoul
>nano pass.sh et j'insere dans le fichier la commande suivante
>cat /etc/bandit_pass/bandit24 > /tmp/rajoul.pass.txt
>cp pass.sh /var/spool/bandit24
apres quelque seconde le pass est dans pass.txt
>cat pass.txt bandit24 : UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ
```
# bandit25
```
#!/bin/bash
pass='UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ'
for i in {1..9}{1..9}{1..9}{1..9}
do
    echo pass $i |nc localhost 30002;
done
>>> bandit25 : uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG
```


