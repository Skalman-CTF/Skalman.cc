---
title: "Houseplant CTF"
date: 2020-04-29T17:19:53+02:00
draft: false
cover: "/images/042020-Houseplant-CTF/Houseplant.png"
Author: "Skalman-Hugo and Skalman-Jimmie"
description: "This was a crazy CTF, organized by [Hack Club](https://hackclub.com) and hosted by [RiceTeaCatPanda](https://riceteacatpanda.wtf). Organized as we are, we never even realized who or what organized this CTF. But apparently Hack Club is the world largest network of high schoolers/students who are in for a game of 'lets blow some shit up' (responsibly that is). Fun!"
toc: true
---
## Houseplant CTF
This was a crazy CTF, organized by [Hack Club](https://hackclub.com) and hosted by [RiceTeaCatPanda](https://riceteacatpanda.wtf). Organized as we are, we never even realized who or what organized this CTF. But apparently Hack Club is the world largest network of high schoolers/students who are in for a game of 'lets blow some shit up' (responsibly that is). Fun!

### CTF Time
* Start: Friday 24-04-2020 21:00 (CET)
* End: Sunday 26-04-2020 21:00 (CET)
* Categories: Beginner, Crypto, Forensics, Misc, OSINT, Pwn, Reverse Engineering, Web

### "Where is Elon?!"
We were focused on a challenge happening on the Discord channel (and a few others), when some of the organizers told us the AMA was going to start. Ehhhh, what AMA? Then there was a random dude shouting "Where is Elon?!", "I want to see Elon".

Still having _no_ clue whatsoever, I continued the challenge when all of a sudden people said Elon Musk was life. Pretty convinced I was being trolled, I took a look at the live stream. All to be greeted by a vaguely familiar face: Elon Musk. Ill be damned.

> “Always take the approach that you are wrong, and try to be less wrong.” — Elon Musk

He even called us a wholesome bunch!

![Elon Musk on the Hack Club AMA](/images/042020-Houseplant-CTF/elon.png "Elon Musk on the Hack Club AMA")

Random? Certainly, but we moved on. If you are interested in the full AMA, there is a [writeup on Teslarati](https://www.teslarati.com/tesla-cybertruck-armor-glass-fail-insights-elon-musk-video/). 

## Challenges

### Beginner 1 through 9
A fun little series of warm-up challenge. Each challenge 1 through 8 all had different types of obfucation, and the final challenge combined all eight. And no, I am not affiliated with CyberChef. But if you don't know it... Check it out!

#### Beginner 1 - Base64
When Bob and Jia were thrown into the world of cybersecurity, they didn't know anything- and thus were very overwhelmed. They're trying to make sure it doesn't happen to you.
Let's cover some bases first.

Challenge:

`cnRjcHt5b3VyZV92ZXJ5X3dlbGNvbWV9`

Command:

`echo "cnRjcHt5b3VyZV92ZXJ5X3dlbGNvbWV9" | base64 -d`

Solution

`rtcp{youre_very_welcome}`

#### Beginner 2 - Hex
Bob wanted to let you guys know that "You might not be a complete failure."
Thanks, Bob.

Challenge:

`72 74 63 70 7b 62 6f 62 5f 79 6f 75 5f 73 75 63 6b 5f 61 74 5f 62 65 69 6e 67 5f 65 6e 63 6f 75 72 61 67 69 6e 67 7d`

Command:
[CyberChef - From Hex](https://gchq.github.io/CyberChef/#recipe=From_Hex('Space')&input=NzIgNzQgNjMgNzAgN2IgNjIgNmYgNjIgNWYgNzkgNmYgNzUgNWYgNzMgNzUgNjMgNmIgNWYgNjEgNzQgNWYgNjIgNjUgNjkgNmUgNjcgNWYgNjUgNmUgNjMgNmYgNzUgNzIgNjEgNjcgNjkgNmUgNjcgN2Q)

Solution:

`rtcp{bob_you_suck_at_being_encouraging}`

#### Beginner 3 - Octal/ASCII
Fun fact: Jia didn't actually know what this was when they first started out. If you got this, you're already doing better than them ;-;

Challenge:

`162 164 143 160 173 163 165 145 137 155 145 137 151 137 144 151 144 156 164 137 153 156 157 167 137 167 150 141 164 137 157 143 164 141 154 137 167 141 163 137 157 153 141 171 77 41 175`

Command:
[CyberChef - From Octal](https://gchq.github.io/CyberChef/#recipe=From_Octal('Space')&input=MTYyIDE2NCAxNDMgMTYwIDE3MyAxNjMgMTY1IDE0NSAxMzcgMTU1IDE0NSAxMzcgMTUxIDEzNyAxNDQgMTUxIDE0NCAxNTYgMTY0IDEzNyAxNTMgMTU2IDE1NyAxNjcgMTM3IDE2NyAxNTAgMTQxIDE2NCAxMzcgMTU3IDE0MyAxNjQgMTQxIDE1NCAxMzcgMTY3IDE0MSAxNjMgMTM3IDE1NyAxNTMgMTQxIDE3MSA3NyA0MSAxNzU)

Solution:

`rtcp{sue_me_i_didnt_know_what_octal_was_okay?!}`

#### Beginner 4 - ROT13
Caesar was stabbed 23 times by 60 perpetrators... sounds like a modern group project

Challenge:

`egpc{lnyy_orggre_cnegvpvcngr}`

Command:
[CyberChef - ROT13](https://gchq.github.io/CyberChef/#recipe=ROT13(true,true,13)&input=ZWdwY3tsbnl5X29yZ2dyZV9jbmVndnB2Y25ncn0)

Solution:

`rtcp{sue_me_i_didnt_know_what_octal_was_okay?!}`

#### Beginner 5 - Morse
beep boop

Challenge:

`-- .- -. -.-- ..--.- -... . . .--. ... ..--.- .- -. -.. ..--.- -... --- --- .--. ...`

Command:
[CyberChef - From Morse Code](https://gchq.github.io/CyberChef/#recipe=From_Morse_Code('Space','Line%20feed')&input=LS0gLi0gLS4gLS4tLSAuLi0tLi0gLS4uLiAuIC4gLi0tLiAuLi4gLi4tLS4tIC4tIC0uIC0uLiAuLi0tLi0gLS4uLiAtLS0gLS0tIC4tLS4gLi4u)

Solution:

`rtcp{MANY_BEEPS_AND_BOOPS}`

#### Beginner 6 - A1Z26
i'm so tired...

Challenge:

`26 26 26 26 26 26 26 26 19 12 5 5 16 9 14 7 9 14 16 8 25 19 9 3 19`

Command:
[CyberChef - A1Z26 Cipher Decode](https://gchq.github.io/CyberChef/#recipe=A1Z26_Cipher_Decode('Space')&input=MjYgMjYgMjYgMjYgMjYgMjYgMjYgMjYgMTkgMTIgNSA1IDE2IDkgMTQgNyA5IDE0IDE2IDggMjUgMTkgOSAzIDE5)

Solution:
`rtcp{zzzzzzzzsleepinginphysics}`

#### Beginner 7 - Atbash Cipher
Don't go around bashing people.

Challenge:

`igxk{fmovhh_gsvb_ziv_nvzm}`

Command:
[CyberChef - Atbash Cipher](https://gchq.github.io/CyberChef/#recipe=Atbash_Cipher()&input=aWd4a3tmbW92aGhfZ3N2Yl96aXZfbnZ6bX0)

Solution:

`rtcp{unless_they_are_mean}`

#### Beginner 8 - Bacon Cipher
You either mildly enjoy bacon, think it's a food of the gods, or are vegan/vegetarian.

Challenge:

`00110 01110 00100 00000 10011 00101 01110 01110 00011 00011 01110 01101 10011 10010 10011 00000 10001 10101 00100`

Command:
[CyberChef - From Octal](https://gchq.github.io/CyberChef/#recipe=From_Octal('Space')&input=MTYyIDE2NCAxNDMgMTYwIDE3MyAxNjMgMTY1IDE0NSAxMzcgMTU1IDE0NSAxMzcgMTUxIDEzNyAxNDQgMTUxIDE0NCAxNTYgMTY0IDEzNyAxNTMgMTU2IDE1NyAxNjcgMTM3IDE2NyAxNTAgMTQxIDE2NCAxMzcgMTU3IDE0MyAxNjQgMTQxIDE1NCAxMzcgMTY3IDE0MSAxNjMgMTM3IDE1NyAxNTMgMTQxIDE3MSA3NyA0MSAxNzU)

Solution:

`rtcp{GOEATFOODDONTSTARVE}`

#### Beginner 9 - Everything combined
Hope you've been paying attention! :D

Challenge:

`MmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMGEgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmQgMmQgMmQgMmQgMmQgMjAgMmUgMmQgMmQgMmQgMmQ=`

![Beginner 9 - combined _everything_](/images/042020-Houseplant-CTF/beginner9.png "Beginner 9 - combined _everything_")

(Whups, forgot to get the right screenshot. But try your best, and combine all of the above. I trust you can! :))

### Reverse Engineering - Fragile
Can you help me move my stuff? This one's fragile!

Challenge:
We were provided with a Java file, printing "Acceess granted." if the correct flag is provided:

```import java.util.*;

public class fragile
{
    public static void main(String args[]) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter flag: ");
        String userInput = scanner.next();
        String input = userInput.substring("rtcp{".length(),userInput.length()-1);
        if (check(input)) {
            System.out.println("Access granted.");
        } else {
            System.out.println("Access denied!");
        }
    }
    
    public static boolean check(String input){
        boolean h = false;
        String flag = "h1_th3r3_1ts_m3";
        String theflag = "";
        if(input.length() != flag.length()){
            return false;
        }
        for(int i = 0; i < flag.length(); i++){
            theflag += (char)((int)(flag.charAt(i)) + (int)(input.charAt(i)));
        }
        return theflag.equals("ÐdØÓ§åÍaèÒÁ¡");
    }
}
```

Solution:
Three variables are used: input, flag and theflag. The function "check" can be described as:

`Every char in the "input" variable is added with the corresponding character in "flag" variable, if it equals ÐdØÓ§åÍaèÒÁ¡ ("theflag" variable) access will be granted`

The final value of "theflag" and "flag" were converted to numbers via RapidTables:

`theflag = 208 100 216 211 153 167 229 146 205 97 232 210 193 161 151`

`flag = 104 49 95 116 104 51 114 51 95 49 116 115 95 109 51`

"theflag" was then subtracted with "flag", this was done with Excel, and then converted to ASCII via RapidTables:

![Reverse Engineering - Fragile Excel solution](/images/042020-Houseplant-CTF/fragile.png "Reverse Engineering - Fragile Excel solution")

Flag:

`rtcp{h3y_1ts_n0t_b4d}`
