# Hacker101 CTF writeup
https://ctf.hacker101.com/ctf

<!-- ![](https://i.imgur.com/bVg4tNv.png)
 -->

## A little something to get you started
### Difficulty: Trivial
### Skills: Web
### Solutions by steps:
- Get in the webpage and open DevTools to see this
![](https://i.imgur.com/6gYTcSU.png)
- It seems that the flag could only hide in the `background.png`

<!-- ANSWER: https://e197ff9f4bbbd9ddd092e1d010fa17ab.ctf.hacker101.com/background.png -->

- After accessing the png file in the webpage, you'll find the flag

<!-- FLAG: ^FLAG^c5af788d5a4a8e7d217e79d701481098a402bb224869f61ce7826287258f731d$FLAG$ -->
- Pass it by pressing `Submit Flag` button on the top bar

## Micro-CMS v1
### Difficulty: Easy
### Skills: Web
### Hint: 
- Try creating a new page
### Solutions by steps:

#### Flag1:
- Create a new page  by typing in any title and contexts
- Look at the URI: `https://XXXXXXXXXX.ctf.hacker101.com/page/10` and guess that there must be some thing hidden in page 1 to 10 
- Press `Edit this page` and `https://XXXXXXXXXX.ctf.hacker101.com/page/edit/THE_NUMBER_YOU_GUESS`
- After a few guessing, you'll get the flag

<!-- FLAG: ^FLAG^ebb1cad68b466eb2c744a8943f0b379aba2e47e907f7f94bd770282264e79110$FLAG$ -->


#### Flag2:
- Press the `Edit this page` button in the post you just created
- Change the title and content to `<svg onload=alert(1)>`
- Press `Go Home` and you'll see the flag

![](https://i.imgur.com/OCNLql5.png)

##### Ref:
https://zhuanlan.zhihu.com/p/107860601

#### Flag3: (SQL injection)
- Add the most common SQL injection `'OR 1=1 --` at `https://XXXXXXXXXX.ctf.hacker101.com/page/edit/HERE`
- Reload the Page to see the flag

<!-- ANSWER: ^FLAG^b6f009ffbecb8b86ee8eeaaea96f6b8e8206dacbbbb55cdc6825b71748038001$FLAG$ -->

#### Flag4: 
- Edit the page you just created and change your content to `<img src="" onerror="alert(1)"/>`
- After updating the screen, open DevTools and find flag in the source code

<!-- ANSWER: ^FLAG^6fef0c8c38ac1aa2f0e4c3ce6d7d5faef7d86583d9cbf571cd67c61b1a01c128$FLAG$ -->






