## List of bad words

<details>
<summary><b>Warning:</b> Bad words, think carefully before clicking</summary>

```py
bad_words = [
# English
# source:
# - http://www.hyperhero.com/en/insults.htm
# - https://reallifeglobal.com/how-to-use-swear-words-in-english/
"ass",
"asshole",
"bitch",
"bullshit",
"butt",
"cock",
"cunt",
"dick",
"fuck",
"fucker",
"motherfucker",
"shit",
"whore",

# Vietnamese
# source: 
# - http://qr.ae/TUp27Z
# - http://qr.ae/TUp27V
# - www.youswear.com/index.asp?language=Vietnamese
"đĩ",
"địt",
"địt mẹ",
"địt bố",
"địt cha",
"địt bà",
"địt cụ",
"chịch",
"cứt",
"đái",
"địt",
"đụ má",
"đéo",
# "bú",
"cặc",
"buồi",
"lồn",
# "lợn" (pig), "chó" (dog)
"vãi đái", 
"vãi cứt", 
"vãi lồn"
]
```

</details>

## Function

```py
def isBadWord(word):
    return word.lower() in bad_words

def isContainingBadWord(s):
    _s = s.lower()
    return any(_s.find(bad_word) != -1 for bad_word in bad_words)
```