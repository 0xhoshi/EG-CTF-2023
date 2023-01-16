# WRITEUP-EG-CTF-2023
---------------------------------------------------------------------------
## __Categories__

- [**OSINT**](#OSINT)
  - [Farewell](#Farewell)
  - [Broken Man](#BrokenMan)
  - [Octopus](#Octopus)
  - [Oldest Historical Tree](#OldestHistoricalTree)
  - [Thirsty](#Thirsty)
  - [SixSenses](#SixSenses)

- [**Web**](#Web)
  - [Japan](#Japan)
  - [Error 500](#Error500)
  - [EVE](#EVE)
  - [Error 404](#Error404)
  - [TutTut](#TutTut)
  - [Birthday](#Birthday)

- [**Reverse Engineering**](#ReverseEngineering)
  - [OldButGold](#OldButGold)
  - [Diamond](#Diamond)
  - [Vault](#Vault)
  - [Complexity](#Complexity)
  - [Ordered](#Ordered)  

- [**Cryptography**](#Cryptography)
  - [WASD](#WASD)
  - [Cartoon](#Cartoon)
  - [DoReMi](#DoReMi)

- [**Steganography**](#Steganography)
  - [CatMeow](#CatMeow)
  - [Mastery](#Mastery)
  - [Class](#Class)

- [**Misc**](#Misc)
  - [Hashcat](#Hashcat)
  - [Mystery Code](#MysteryCode)
  - [SuperBrain](#SuperBrain)
  - [MysteryBunny](#MysteryBunny)

- [**Networking**](#Networking)
  - [IPV4](#IPV4)
  - [IPV6](#IPV6)
  - [AirDream Network](#AirDreamNetwork)

- [**Forensics**](#Forensics)
  - [Corrupted](#Corrupted)
  - [Signal](#Signal)
  - [AutoBot](#AutoBot)
  - [Broken Oyen](#BrokenOyen)

- [**Programming**](#Programming)
  - [Rigorous](#Rigorous)

---------------------------------------------------------------------------

## OSINT
### Farewell
![Farewell chal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/Screenshot%202023-01-16%20213043.png?raw=true)

For this challenge, we were given a letter that looks like this : -

![letter](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-16%20222141.png?raw=true)

As you can see, at the end of the letter, we were provided with a phone number that belongs to Syahirah's boyfriend maybe?

Out of curiousity, I searched for his number in an application called GetContact and just like that I found the flag :

![getcontact](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/msg-763160323-59716.jpg?raw=true)

flag : -
```
EG{g3t_3xp0s3d}
```


### Broken Man
![BrokenMan chal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/Screenshot%202023-01-16%20213057.png?raw=true)

As you can see in the chal description, it says ```@theniceguy4485 1 year ago``` what could this be? maybe it will be useful later

We were provided with a picture of a particular youtube videos with a length of ```3:29``` : -

![brokenmanpng](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/brokenFlag(1).jpg?raw=true)

After doing some research, I found out that the character showed in the image is from a show called 'Peaky Blinders'.

I searched for ```Peaky Blinders Broken Man``` and found the exact video that looks like the image provided

![youtubevideo](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-16%20225154.png?raw=true)

I scrolled down the comment section and found a comment from ```The Nice Guy```, sounds familiar right? I read the reply section of the comment and found a reply by EliteGhost MY that looks like an Base64 Encoded text.

![egcomment](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-16%20225227.png?raw=true)

decode the text and got the flag.

flag : -
```
EG{K33P_GR1ND1NG}
```


### Octopus
![Octopus chal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/Screenshot%202023-01-16%20213108.png?raw=true)

They provide us with an image of ```OctoCat``` or well known as the mascot of ```GitHub```

![octocat](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/code(1).jpg?raw=true)

Nothing looks suspicious in this image, so I use [hex editor](https://hexed.it/) to check the content of the image, scrolled down and found what it looks like a Base64 Encoded text

![hexeditor](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-16%20231031.png?raw=true)

decoded it and we got a text that says : -
```0hanif0/EGCTF2023```

So I searched for ```0hanif0``` in GitHub and try to find a repository named ```EGCTF2023```

At the time im writing this writeup, ```0hanif0``` already deleted the repository, So I cant show how it exactly being done, sorry about that

BUT, of course I remember how I got trolled when opened the ```EGCTF2023``` repository instead of flag. >: (

After check the commits of the repository, I found the flag that is written upside down. : )

flag : -
```
EG{G1THUB_1S_FUN}
```


## Oldest Historical Tree
![oldesthistoricaltree](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/Screenshot%202023-01-16%20213120.png?raw=true)

This is one of the challenge that i found to be very interesting,

We were given a link to a ["Tempat Menarik di Ipoh"](https://www.caridestinasi.com/tempat-menarik-ipoh/) and an image of a Pokemon Go map that is supposed to be somewhere in Ipoh.

![pokemongo](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/memories(2).jpg?raw=true)

After an extensive time of searching a place that looks like the image given, I found a place that does looks similar to the image, the place is ```Dataran KTM Ipoh```

![gambardataran](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-16%20235232.png?raw=true)

I decide to scroll down the image section of ```Dataran KTM Ipoh``` in Google Maps and found an [image](https://www.google.com/maps/place/Dataran+KTM+Ipoh/@4.5971665,101.0738315,3a,75y,90t/data=!3m8!1e2!3m6!1sAF1QipNTAXfBHnmXv9fw8mNoxuTvMX7jIup5VTVnNr2T!2e10!3e12!6shttps:%2F%2Flh5.googleusercontent.com%2Fp%2FAF1QipNTAXfBHnmXv9fw8mNoxuTvMX7jIup5VTVnNr2T%3Dw203-h404-k-no!7i591!8i1178!4m7!3m6!1s0x31caec7faab3f6c3:0x1eae66eaff84acff!8m2!3d4.5971665!4d101.0738315!14m1!1BCgIgARICGAI) uploaded by XioN that looks exactly like the image given in the challenge : -

![pokemonimage](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-16%20235847.png?raw=true)

At the bottom of the image, there is a link that directs to EliteGhost Facebook account

Looking at the latest post, There is an account commented a link to a video of pikachu dancing or something? sus.

![facebookpost](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20000112.png?raw=true)

I check that pikachu-themed facebook account and scroll al the way down to the oldest post to find a picture of ```tree``` with a caption ```"Old Tree"```

![treepost](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20000638.png?raw=true)

![tree](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/320940859_703689328058780_5696869565390281112_n.jpg?raw=true)

I noticed a weird-looking text at the top-right of the image that is written in flag format

Luckily, I have seen this kind of cipher called ```Old Krytan``` in [```H0j3n GitHub```](https://github.com/H0j3n/EzpzCTF)


Decoded it and I obtained the flag

flag : -
```
EG{L0T5_0F_M3M0R135}
```


## Thirsty
![thirsty chal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/Screenshot%202023-01-16%20213132.png?raw=true)

Long story short, Pikachu wants Starbucks's Frappuccino.

We were given three materials that is ```Menu.zip```, ```Place.zip``` that requires password and ```pokemon.jpg```

```pokemon.jpg``` is an image of Pokemon Go map just like ```Oldest Historical Tree``` but with different place.

![medangopeng](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/pokemon(2).jpg?raw=true)

I searched for ```Starbucks in Ipoh``` in Google Maps and the first place that showed up was Starbucks Ipoh Parade, but the map's terrain doesn't seem similar as the image provided

The second place that showed up was ```Starbuck Medan Gopeng``` and the terrain does looks similar to the image given.

I attempt to input ```Starbucks Medan Gopeng``` as a password to ```Place.zip``` and it works !!

Place.zip Password : -
```
Starbucks Medan Gopeng
```

It contains an image to someone's Instagram feed, judging by the image given, this "someone's" account is following eliteghostmy Instagram account

![pngnya](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/photo_2023-01-11_19-08-09.jpg?raw=true)

So i scrolled through the list of eliteghostmy followers an trry to find an account that have the same profile pics as the one in the image.

![instadia](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20005051.png?raw=true)

Found it !! the account is [nnshuhada._ ](https://www.instagram.com/nnshuada._/)

The account only have one post that shows a picture of Pikachu sitting(?) besides a cup of Starbucks Coffee (how cute)

And above the Starbucks cup there is a caption that says ```MOCHAPRALINEFRAPPUCCINO``` (how do you even pronounce this, seriously)

that soundS like a menu name to me, So i try to use it as a password to ```Menu.zip``` and yes, it works.

Menu.zip Password : -
```
MOCHAPRALINEFRAPPUCCINO
```

The zip file contains one video file and one text file

The video file is a pokemon song with an image that looks like this : -

![lagupokemon](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20005739.png?raw=true)

While the text file is the lyrics to that pokemon song : -
```
I wanna be the very best
Like no one ever was
To catch them is my real test
To train them is my cause
I will travel across the land
Searching far and wide
Each Pokemon to understand
The power that's inside!
Pokemon!
Gotta Catch 'em all!
It's you and me
I know it's our destiny
Pokemon!
Oh, you're my best friend
In a world we must defend!
Pokemon!
Gotta catch 'em all!
A heart so true
Our courage will pull us through!
You teach me and I teach you
Pokemon!
Gotta Catch 'em all!
Gotta Catch 'em all!
Oh yeah...
Every challenge along the way
With courage i will face
I will battle every day
To claim my rightful place!
Come with me, the time is right
There's no better team
On and On we'll win the fight
It's always been our dream
Pokemon!
Gotta Catch 'em all!
It's you and me
I know it's our destiny
Pokemon!
Oh, you're my best friend
In a world we must defend!
Pokemon!
Gotta catch 'em all!
A heart so true
Our courage will pull us through!
You teach me and I teach you
Pokemon!
Gotta Catch 'em all!
Gotta Catch 'em all!
Gotta Catch 'em all!
Gotta Catch 'em all!
Gotta Catch 'em all!
Yeah!
Pokemon!
Gotta Catch 'em all!
It's you and me
I know it's our destiny
Pokemon!
Oh, you're my best friend
In a world we must defend!
Pokemon!
Gotta catch 'em all!
A heart so true
Our courage will pull us through!
You teach me and I teach you
Pokemon!
Gotta Catch 'em all!
Gotta Catch 'em all!
Pokemon!
```

What is that weird-looking number format on the right side? yes, it's a [Book Cipher](https://en.wikipedia.org/wiki/Book_cipher)

Huh? You don't know how Book Cipher works? ** sigh **

Take for example the first line of the book cipher that is : -
```
12 : 5 : 2
```

So how it works is like this, the first number refers to the ```line```

From the text provided, what is the ```12th``` line? it is : -
```
I know it's our Destiny
```

the second number refers to the ```words```

The ```5th``` words is ```Destiny```

And the third number refers to the ```alphabet```

The ```2nd``` alphabet in ```Destiny``` is ```E```

Yayy !! you decoded the first alphabet of the flag !! 15 more to go ╥﹏╥

Decoded it and I obtained the flag

flag : -
```
EG{REST_WITH_COFFEE}
```


## SixSenses
![sixsenses chal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/Screenshot%202023-01-16%20213156.png?raw=true)

Apart from ```Oldest Historical Tree```, This is another challenge that I found to be very interesting

They provide us with an image of what is seems to be is a cipher based on sign language

![bahsaisyarat](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20012132.png?raw=true)

I searched for [sign language cipher](https://www.dcode.fr/american-sign-language) and decoded it

It appears to be a domain that contains mp3 file : -
```
https://eliteghost.tech/lalala.mp3
```
After distinctly listening to it multiple times, There is a subtle voice that says ```"Cari Aiman di Followers EliteGhost Instagram"``` from ```2:08``` to ```2:15```

So... I guess I need to cari Aiman in order to get the flag then?

Then I found this handsome [aiman](https://www.instagram.com/aimantinoo22/) and it contains some highlights and posts which is useful to obtain the flag

![aiman](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20013922.png?raw=true)

The first highlights contains a link that directs to [this link](https://eliteghost.tech/eye.jpg): -
```
https://eliteghost.tech/eye.jpg
```
what could this be? sixth sense maybe?


The second highlights shows an order on how to get the flag right : -

![order](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20014523.png?raw=true)

We already got an ```eye```, the remaining are ```ear```, ```tongue``` and ```nose```

### Ear

![telinga](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20014830.png?raw=true)

This one is the most direct, You can see the post contain an image of ear with caption  ```_S3NS3```

The second part of the flag is : -
```
_S3NS3
```

### Tongue

![lidah](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20020321.png?raw=true)

Notice how Aiman highlights or posts doesnt contain anything related to tongue? That's why i decide to search for his following and found this [account](https://www.instagram.com/izzkhamilia/) and yes it does have tongue picture like i showed above

The order is ```sweet sour salty bitter``` which is a part of taste buds : -

![tastebuds](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20020748.png?raw=true)

The cipher is ancient egypt hieroglyphs cipher : -

![egypt hieroglyphs](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/687474~1.JPE?raw=true)

Decode it and we get the third part of the flag : -
```
IS_SO
```
### Nose

![hidung](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20015210.png?raw=true)

Back to aimantino22, The post contain an image of nose with a caption that appears to be an esoteric language called [Brainfxck](https://en.wikipedia.org/wiki/Brainfuck)

Decode it to plain text an we get ```R3}```

But that doesn't seems like a complete word, if you observe the image thoroughly, there is actually a written text that is ```R4```

Combine it and we got the fourth part of the flag : -
```
R4R3}
```

Combine all parts with an order of ```eye, ear, tongue, nose``` and we got the flag.

flag : -
```
S1X_S3NS3_IS_SO_R4R3}
```
