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
  - [Error 500](#Error-500)
  - [EVE](#EVE)
  - [Error 404](#Error-404)
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
  - [Doraemon](#Doraemon)
  - [DoReMi](#DoReMi)
  - [NATO](#NATO)

<!--- [**Steganography**](#Steganography)
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
  - [Broken Oyen](#BrokenOyen)-->

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


### Thirsty
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


### SixSenses
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

#### Ear

![telinga](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/OSINT/MATERIAL/Screenshot%202023-01-17%20014830.png?raw=true)

This one is the most direct, You can see the post contain an image of ear with caption  ```_S3NS3```

The second part of the flag is : -
```
_S3NS3
```

#### Tongue

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
#### Nose

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
EG{S1X_S3NS3_IS_SO_R4R3}
```

---------------------------------------------------------------------------

## Web
### Japan

![japanchal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/Screenshot%202023-01-16%20212415.png?raw=true)

This challenge provide us with a link to a Japan website that is [jprs.jp](https://jprs.jp/) and a pdf file called ```admin-sign-3.pdf``` that requires password.

Using [whois](https://www.whois.com) website I managed to find the admin sign-key that is : -
```
4D06600DDB3967F38997FA74706624E3DB15159464A4F0E4C27F7DABC8E0E7A6
```

Use it as a password to ```admin-sign-3.pdf``` and we can access the pdf, the flag is contain inside the file.

flag : -
```
EG{WH01S_L00KUP_1S_34SY}
```


### Error 500

![error500chal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/Screenshot%202023-01-16%20212457.png?raw=true)

We were provided with a [domain](https://eliteghost.tech/unknown/) that is : -
```
https://eliteghost.tech/unknown/
```
The flag is in the website and is written in white text to make it invisible, so you need to inspect it in order to get the flag.

![patutnya](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/MATERIAL/Screenshot%202023-01-17%20024748.png?raw=true)

Luckily, I have dark reader extension so i got the flag right away just like that

![takpatut](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/MATERIAL/Screenshot%202023-01-17%20024814.png?raw=true)

flag : -
```
EG{G1nZ_1s_H3r3}
```


### EVE

![wechal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/Screenshot%202023-01-16%20212517.png?raw=true)

We were provided with a [link](https://eliteghost.tech/wall-e/) that will make you feel lonely : -
```
https://eliteghost.tech/wall-e/
```

Even the Robot Already has a partner? Seriously? me when : (

And yes, as you can see the hint is already there, its about robot

So I try to get the list of directories using ```robots.txt``` the link will look like this : -
```
https://eliteghost.tech/wall-e/robots.txt
```

I look for directory that have weird name and found this Base64 Encoded directory : -
```
/czNjcjN0MTMzNw==
```

looks pretty weird to me, after decode it we get the plain text that is ```s3cr3t1337```

I go to this directory in attempt to find the flag : -
```
https://eliteghost.tech/wall-e/s3cr3t1337
```

Just like ```Error 500``` chal, You supposed to to inspect it in order to get the flag. Lucky me I have dark reader extension so I got the flag right away but is is Base64 Encoded

![pages3cr3t](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/MATERIAL/Screenshot%202023-01-17%20030456.png?raw=true)

Decode it and we get the flag.

flag : -
```
EG{R0B0tS_W1tH_B64_Wa5_So_FXN_R1GHT}
```


### Error 404

![error404chal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/Screenshot%202023-01-16%20212540.png?raw=true)

This challenge provide us with this [link](https://eliteghost.tech/genuine/index.html) : -
```
https://eliteghost.tech/genuine/index.html
```

The page have multiple hyperlink text that directs to different things and I just open all the links possible

One of the hyperlink text that states ```Description``` directs to a [link](https://eliteghost.tech/genuine/anepp.html) that says "Maybe Flag?" with a text that looks like Base64 Encoded : -
```
UlVkN1NsVTFOMTlMTVVSRU1VNUhmUT09
```

Decode it two times and we got the flag.

flag : -
```
EG{JU57_K1DD1NG}
```


### TutTut

![tututchal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/Screenshot%202023-01-16%20212600.png?raw=true)

This challenge provide us with an image that shows a morse code for numbers and a link

![gamabr](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/MATERIAL/morsecode(2).png?raw=true)

Go to the [link](https://eliteghost.tech/IV.html) and it says : -
```
The flag is not here, Try again!
```

The html file is written in Roman number that represents number ```4```

Convert the Roman number to morse code by referring the image given and it will look like this : -
```
https://eliteghost.tech/....-.html
```

The flag is written on that page

flag : -
```
EG{L34RN_M0RS3_C0D3}
```


### Birthday

![bedaychal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/Screenshot%202023-01-16%20212617.png?raw=true)

This challenge provide us with one zip file, ```present.zip``` that requires password

The hint is in the challenge itself
```
I mean, EliteGhost was here since 10's. But what about eliteghost.tech?
```

So I looked up [domain age checker](https://smallseotools.com/domain-age-checker/) and found out that eliteghost.tech was established on 12/10/2022

Use that as a password to the zip file but in YYYY/MM/DD format, and it opened

```present.zip``` password : -
```
20221012
```

From the file, we obtained an image that is a poster of EGCTF2023 but there is nothing suspicious in the image.

So I bring up [aperisolve.com](https://www.aperisolve.com) to know more in details about the image provided.

There is quite a bit of text in this Zsteg section 

![zsteg](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/MATERIAL/Screenshot%202023-01-17%20033803.png?raw=true)

Look thoroughly and found the flag : -

![falgzst](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/WEB/MATERIAL/Screenshot%202023-01-17%20033841.png?raw=true)

flag : -
```
eg{h4ppy_n3w_y34r_ctf_2023}
```


---------------------------------------------------------------------------

## Reverse Engineering
### OldButGold

![oldbutgold](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/REVERSE%20ENGINEERING/Screenshot%202023-01-16%20212147.png?raw=true)

This challenge provide us with one text file that contains as below : -
```
subroutine check_password(input, result)
  implicit none
  character(len=*), intent(in) :: input
  logical, intent(out) :: result
 
  integer, parameter :: defcon(18) = [51, 76, 49, 84, 51, 71, 72, 48, 83, 84, 95, 52, 67, 52, 68, 51, 77, 89]
  character(len=1) :: input_char
  integer :: input_char_code
  logical :: correct
  
  correct = .true.
  do i = 1, len(input)
    input_char = input(i:i)
    input_char_code = int(input_char)
    if (input_char_code - defcon(i)).abs /= 1 then
      correct = .false.
      exit
    end if
  end do
  result = correct
end subroutine check_password

program test
  implicit none
  
  character(len=*), parameter :: password_prompt = "Enter password:"
  character(len=*), parameter :: defconx = "Now that's the flag! Put it with EG{}"
  character(len=*), parameter :: incorrect_message = "Incorrect password."
  character(len=*), parameter :: password
  logical :: is_correct
  
  write(*,*) password_prompt
  read(*,*) password
  
  call check_password(password, is_correct)
  
  if (is_correct) then
    write(*,*) defconx
  else
    write(*,*) incorrect_message
  end if
end program test
```

Line of code that got my attention in this text file is : - 
```
integer, parameter :: defcon(18) = [51, 76, 49, 84, 51, 71, 72, 48, 83, 84, 95, 52, 67, 52, 68, 51, 77, 89]
```

That does looks like ASCII representation of character

Using online [ASCII to text converter](https://www.duplichecker.com/ascii-to-text.php) and I got the flag

flag : -
```
EG{3L1T3GH0ST_4C4D3MY}
```


### Diamond

![diamondchal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/REVERSE%20ENGINEERING/Screenshot%202023-01-16%20212209.png?raw=true)

This challenge provide us with a file that is written in Ruby, The content of the file looks like this : -
```
def rot13(s)
    k = "N-ZA-Mn-za-m"
    return s.tr("A-Za-z", k)
  end
  
  def c(p)
    e = "F0_gu1f_1f_e0g13_J3yp0zr"
    d = rot13(e)
    if p == d
      puts "Correct password, here's your flag! : EG{#{d}}"
    else
      puts "Wrong password"
    end
  end
  
  print "Enter password: "
  password = gets.chomp
  
  c(password)
  ```
  
  I see ```rot13```, I see ```"F0_gu1f_1f_e0g13_J3yp0zr"```, I [decode](https://rot13.com/), I got flag : )
  
  flag : -
  ```
  EG{S0_th1s_1s_r0t13_W3lc0me}
  ```
  
  
  ### Vault
  
  ![vaultchal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/REVERSE%20ENGINEERING/Screenshot%202023-01-16%20212225.png?raw=true)
  
  This challenge provide us with a text file ```passcode.txt``` and a zip file ```vault.zip``` that require password obtained from ```passcode.txt```
  
  ```passcode.txt``` content looks like this : -
  ```
  x = 1337
y = x % 882726
z = int(str(y)[::-1])
a = z * y
g = x + y + z + a
passcode = (x + g + y + z + a) * 2
```

just calculate it normally and you will get the passcode : -
```
y = x % 882726
   = 1337 % 882726
   = 1337
z = 7331
a = 7331 * 1337 = 9801547
g = 1337 + 1337 + 7331 + 9801547 = 9811552
passcode = (1337 + 9811552 + 1337 + 7331 + 9801547) * 2 

= 39246208
```

```vault.zip``` password : -
```
39246208
```

flag : -
```
EG{M4THS_1S_FUN}
```

### Complexity

![complexitychal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/REVERSE%20ENGINEERING/Screenshot%202023-01-16%20212252.png?raw=true)

This challenge provide us with a file that is written in Java and all you need is patience ; )

The code is just a bunch of nonsense, you need to locate the flag that was hid somewhere in the code

Using my eagle eye, I manage to locate the flag that is Base64 Encoded : -

![gambarbukti](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/REVERSE%20ENGINEERING/Screenshot%202023-01-17%20040717.png?raw=true)

```
REZ7U0czUTNfMVJfNEtWNFhSX0VLNFZ9
```

You will need to decode it two times in order to get the flag, Base64 than ROT

flag : -
```
EG{TH3R3_1S_4LW4YS_FL4W}
```


### Ordered

![orderdechal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/REVERSE%20ENGINEERING/Screenshot%202023-01-16%20212314.png?raw=true)

This challenge provide us with a file that is written in C++ that looks like this : -
```
#include <iostream>

int main() {
    char A = 1 + 0;
    char E = H + 5;
    char B = E + 2;
    char J = "}" + 10;
    char F = 4 + 6;
    char I = R + 9;
    char D = "{" + 4;
    char G = X + 7;
    char C = G + 3;
    char H = 0 + 8;
    char FLAG = "?";
    }
```

I dont know how to explain this, but the pattern is actually pretty obvious. Notice how ```A``` have ```1``` and ```B``` have ```2```?

Lets list them in alphabetical order

```
    char A = 1 ;
    char E = 5;
    char B = 2;
    char J = 10;
    char F = 6;
    char I = 9;
    char D = 4;
    char G = 7;
    char C = 3;
    char H = 8;
```

Maybe now you can see better? Notice how you can arrange them from ```1(A)``` to ```10(J)``` ?

```
    char A = 0 + 1;
    char B = E + 2;
    char C = G + 3;
    char D = "{" + 4;
    char E = H + 5;
    char F = 4 + 6;
    char G = X + 7;
    char H = 0 + 8;
    char I = R + 9;
    char J = "}" + 10;
```
Andd done, we obtained the flag

flag : -
```
EG{H4X0R}
```

### Vault 2.0

![vault2.0chal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/REVERSE%20ENGINEERING/Screenshot%202023-01-16%20212332.png?raw=true)

This challenge provide us with a text file ```passcode.txt``` and zip file ```flag.zip``` that requires password

The content of ```passcode.txt``` looks like this : -
```
HAI 1.2CAN H…BYE
UNV->;?PN[-UN`-`aQV\LV-UN`-N-N-Vag->@@DV-UN`-N-O-Vag-D@@>V-UN`-N-P-Vag->E?@V-UN`-N-Q-Vag-?D@CV-UN`-N-R-Vag-?@D=V-UN`-N-S-Vag-FFFFV-UN`-N-]N``P\QR]N``P\QR-_-`bZ-\S-N-N[-O9-QVSS-\S-P-N[-Q9-]_\QbXa-\S-N-N[-O9-^b\`Ub[a-\S-R-N[-ScV`VOYR-/aur-}n☺☺p|qr-v☺G-/-N[-]N``P\QRV-UN`-N-e-Vag-@;>AVZ-V[-f_-Y\\]-b]]V[-f_-e-aVY-O\aU-`NRZ-e-N[-A;>A--VZ-V[-f_-Y\\]-b]]V[-f_-e-aVY-O\aU-`NRZ-e-N[-A;>A--f_-e-_-`bZ-\S-e-N[-=;=>VZ-\baaN-f_-Y\\]TVZZRU-eXaUeOfR
```

What in the world is that...

The first line states : -
```
HAI 1.2CAN H…BYE
```

This is a hint that this entire gibberish-looking text is actually a code written in [LOLCODE](http://www.lolcode.org/) because every LOLCODE program will start with ```HAI 1.2 CAN HAS STDIO?``` and end with ```KTHXBYE```

After doing some research, The code is encoded in ASCII +13 shift cipher, after decode it we will get : -
```
HAI 1.2
CAN HAS STDIO?
I HAS A A ITZ 1337
I HAS A B ITZ 7331
I HAS A C ITZ 1823
I HAS A D ITZ 2736
I HAS A E ITZ 2370
I HAS A F ITZ 9999
I HAS A PASSCODE
PASSCODE R SUM OF A AN B, 
DIFF OF C AN D, 
PRODUKT OF A AN B, 
QUOSHUNT OF E AN F
VISIBLE 'passcode
```

To make it easier, Lets break up the code and calculate it manually

```
A = 1337
B = 7331
C = 1823
D = 2736
E = 2370
F = 9999
PASSCODE =
SUM OF A AND B (A + B) = 8668
DIFF OF C AND D (C - D) = -913
PRODUKT OF A AN B (A * B) = 9801547
QUOSHUNT OF E AN F (2370 / 9999) = 0.2370237
```

The description already stated how the format of the passcode should be that is : -
```
xxxx--xxx-xxxxxxx-x.xxxxxxx
```

Insert the number we obtained from the calculation sequentially

```flag.zip``` Password : -
```
8668--913-9801547-0.2370237
```

flag : -
```
EG{4LW4YS_G3T_TR0LL3D}
```


---------------------------------------------------------------------------

## Cryptography
### WASD

![wasdchal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/CRYPTOGRAPHY/Screenshot%202023-01-16%20211940.png?raw=true)

This challenge provide us with a text file ```flag.txt``` that contains this cipher: -
```
WFPA2XE2R)X9S2{
```

From the challenge description, It is obvious that this use [Keyboard Shift Cipher](https://www.dcode.fr/keyboard-shift-cipher)

Decode it and we get the flag

flag : -
```
EG{S3CR3T_C0D3}
```


### Cartoon

![cartoonchal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/CRYPTOGRAPHY/CARTOON/Screenshot%202023-01-16%20212011.png?raw=true)

This challenge provide us with an image of weird-looking cipher

![pelik](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/CRYPTOGRAPHY/CARTOON/flag(5).png?raw=true)

So I searched up weird-looking cipher (literally) and found [this](https://www.dcode.fr/dancing-men-cipher)

The Cipher is actually named Dancing Men Cipher

Decode it and we get the flag

flag : -
```
EG{UNBELIEVABLECIPHER} 
```


### Doraemon

![doraemonchal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/CRYPTOGRAPHY/DORAEMON/Screenshot%202023-01-16%20212126.png?raw=true)

This challenge provide us with an image of weird-looking cipher (again)

![peliklagi](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/CRYPTOGRAPHY/DORAEMON/flag(5).png?raw=true)

Luckily, I came across this cipher while searched up for ```Cartoon``` and this cipher is called [Dorabella Cipher](https://www.dcode.fr/dorabella-cipher)

Decode it and we get the flag

flag : -
```
EG{DORABELLACHPHER}
```

### DoReMi

![doremichal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/CRYPTOGRAPHY/DOREMI/Screenshot%202023-01-16%20212043.png?raw=true)

This challenge provide us with an image of what it looks like is a music sheet 

![musicsheet](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/CRYPTOGRAPHY/DOREMI/flaggg(1).jpg?raw=true)

I found this decoder called [Music Sheets Decoder](https://www.dcode.fr/music-sheet-cipher) and use it to decode the message in the image provided

flag : -
```
EG{IFMUSICWASINCODE}
```

### NATO

![nato](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/CRYPTOGRAPHY/Screenshot%202023-01-16%20212107.png?raw=true)

This challenge provide us with a text file that contains a cipher
```
EG{Romeo Oscar Golf Echo Romeo Tango Hotel Alpha Tango Sierra India Romeo}
```
Definitely always hear this while watching an action movies

As the the title suggests, its a alphabet phonetic in NATO

![gambarnato](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/CRYPTOGRAPHY/GettyImages-1060490970-dcac66d9cda841638d49bc10f5dc1a8b.jpg?raw=true)

Decode it and we get the flag

flag : -
```
EG{ROGERTHATSIR}
```


---------------------------------------------------------------------------

## Programming
### Rigourous

![riguruschal](https://github.com/kanezare/EG-CTF-2023/blob/main/CHALLENGE/PROGRAMMING/Screenshot%202023-01-16%20211908.png?raw=true)

This challenge provide us a zip file ```flag.zip``` that contains 4 main text files that is : -
```
[^a-zA-Z0-9_].apk.txt:

^(\\S+)\\s+(\\S+)$ || D'`;M#8n<;G3zx6Te@,PqMo:n%*#(4hffBA.~}+{)9rqvutsl2pohPle+ihJIedcb[!_^@VUTYRQPtTSRQ3ONGkjW

[^a-zA-Z0-9_].ipa.txt:

^(\\S+)\\s+(\\S+)$ || D'``_9"n[HX9ih6fe3,sN)LoJ87jGX~DeASc~a_N):rqvutsl2johgfkjc)gIH^]\"`_A@\Uy<;QPt76LpP2NMLKDhHGF?>bO

[^a-zA-Z0-9_].exe.txt:

^(\\S+)\\s+(\\S+)$ || D'`%_9"=[l:{8VC54uQ>0).:]%$ki!g21{"cx}O<)srwp6tsrkpongf,jiKgf_%F\[`_^]VzZ<;WVOsMRQJnH0LEJCBf)?DC<;_L

[^a-zA-Z0-9_].osx.txt:

^(\\S+)\\s+(\\S+)$ || D'`N@9>~ZZXXyV6Tuu2rNM;:&+H6GiWfBTzcaP|N)y[wpunsl2pohglkjiba'edFb[!_^@?UTxRQPOTSLpP2NMLEDhU
```

and a ```formula.txt``` that seems to be an arrangement for the 4 main files : -
```
apk: f(x) = sin(x^2 + 1) + 1
ipa: 2
exe: 3
osx: 4
```

f(x) = sin(x^2 + 1) + 1 is equal to 1, So 
```
apk: 1
ipa: 2
exe: 3
osx: 4
```
As you can see from the 4 main files, there is a useless Regular Expressions at the start of the statement : ```^(\\S+)\\s+(\\S+)$ ||```

Delete this on every file and we will get
```
[^a-zA-Z0-9_].apk.txt:

D'`;M#8n<;G3zx6Te@,PqMo:n%*#(4hffBA.~}+{)9rqvutsl2pohPle+ihJIedcb[!_^@VUTYRQPtTSRQ3ONGkjW

[^a-zA-Z0-9_].ipa.txt:

D'``_9"n[HX9ih6fe3,sN)LoJ87jGX~DeASc~a_N):rqvutsl2johgfkjc)gIH^]\"`_A@\Uy<;QPt76LpP2NMLKDhHGF?>bO

[^a-zA-Z0-9_].exe.txt:

D'`%_9"=[l:{8VC54uQ>0).:]%$ki!g21{"cx}O<)srwp6tsrkpongf,jiKgf_%F\[`_^]VzZ<;WVOsMRQJnH0LEJCBf)?DC<;_L

[^a-zA-Z0-9_].osx.txt:

D'`N@9>~ZZXXyV6Tuu2rNM;:&+H6GiWfBTzcaP|N)y[wpunsl2pohglkjiba'edFb[!_^@?UTxRQPOTSLpP2NMLEDhU
```

The statement above is actually a code written in esoteric programming language called Malbolge, So if we execute the code one by one using [Malbolge Compiler](https://www.tutorialspoint.com/execute_malbolge_online.php) and combine it together we will get the flag that is Base64 Encoded
```
RUd7TTRMQjBMRzNfMVNfSDRSRH0=
```

Decode it and we get the flag

flag : -
```
EG{M4LB0LG3_1S_H4RD}
```
