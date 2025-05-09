*Сложность: лёгкая*
## Как решать?
1. ` binwalk redflaggggggggg.png `
2. ` binwalk -e redflaggggggggg.png `
3. 
    ```
    wget https://raw.githubusercontent.com/openwall/john/bleeding-jumbo/run/7z2john.pl

    chmod +x 7z2john.pl

    ./7z2john.pl redflag.7z > 7z_hash.txt 
    ```
4. ` john --format=7z --wordlist=/usr/share/wordlists/rockyou.txt 7z_hash.txt `

> password: booboo

5. Декодировать base64 и найти флаг: flag{5teg4noBB4se64}
