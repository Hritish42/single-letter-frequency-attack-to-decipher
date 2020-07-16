## Single-letter-frequency-attack-to-decipher


Cryptography Challenge 1.

Use single letter frequency attack to decipher the the following message.You know that it has been created with an additive (Shift) cipher. PXPXKXENVDRUXVTNLXHYMXGMAXYKXJNXGVRFXMAHWGXXWLEHGZXKVBIAXKMXQM . 

I've Used Python 3 For solving Challenge


## Usage

```python
message='PXPXKXENVDRUXVTNLXHYMXGMAXYKXJNXGVRFXMAHWGXXWLEHGZXKVBIAXKMXQM'
LETTERS='ABCDEFGHIJKLMNOPQRSTUVWXYZ'
FREQ='ETAOINSHRLDCUMWFGYPBVKJXQZ'
box=''
box2=[]
j=0
for q in FREQ:
w=LETTERS.find(q)
key=0
box2.append(w)
w=key
print('KEYS:-'+str(box2)+'\n\n\n DECRYPTION:-')
for key in box2:
if len(box)==len(message):
j=j+1
print('***'*10)
print(box)
box=''
for x in message:
y=LETTERS.find(x)
d=(y-key)%26
a=LETTERS[d]
box=box+str(a)

```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
