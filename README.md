# Find Hidden Treasure

$ regexs=$(curl -s 'https://raw.githubusercontent.com/ibnufachrizal/JS-Hunt/main/file.txt'|tr '\n' '|')

$ cat yourfile_js.txt | while read url; do python3 ~/SecretFinder/SecretFinder.py -i $url -o cli -r "\w+($regexs)\w+" >> result_secret.txt ;done

**𝐔𝐬𝐢𝐧𝐠 "𝐠𝐫𝐞𝐩" 𝐭𝐨 𝗘𝘅𝘁𝗿𝗮𝗰𝘁 𝗨𝗥𝗟'𝘀 𝗳𝗿𝗼𝗺 𝗷𝘂𝗻𝗸 𝗱𝗮𝘁𝗮**

* 'cat file | grep -Eo "(http|https)://[a-zA-Z0-9./?=_-]*"*'
* 'curl http://host.xx/file.js | grep -Eo "(http|https)://[a-zA-Z0-9./?=_-]*"*'
