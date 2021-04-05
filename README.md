# Find Hidden Treasure

$ regexs=$(curl -s 'https://raw.githubusercontent.com/ibnufachrizal/JS-Hunt/main/file.txt'|tr '\n' '|')

$ cat yourfile_js.txt | while read url; do python3 ~/SecretFinder/SecretFinder.py -i $url -o cli -r "\w+($regexs)\w+" >> result_secret.txt ;done
