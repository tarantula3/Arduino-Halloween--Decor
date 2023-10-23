# Arduino Halloween Decor

3D Printed Arduino Halloween Décor 
---------------------------------
[![Hxfhwr0Eoqk](https://i.imgur.com/DDCVjuD.png)](https://youtu.be/Hxfhwr0Eoqk)

When the full moon is shining and the wolves are howling, it's time for Halloween's spooky spectacle. The snickering grins of jack-o'-lanterns glow from lit porches. Kids skip down the block in spooky costumes, carrying bags full of candy and shouting "Trick or Treat!". The Nightmare Before Christmas is almost here...
Do you see dead people???

Alright Enough of that, in this Spooktacular video I am going to create an Arduino based 3D printed Halloween Décor.
It's super easy, fun and spooky....


3D Printing 
-----------
![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhoKJkcm6gxSypdYdQS9YZp7ufNiU_i-wLdQo3tUBUR9Odynym9QU7As03wcqw_26o5_ImIFnrwgYTO-xXMKAyce-52fK-zv6GFDTR3PiGUgb5Kw9Fbh7UvFob4fq7_igZu8iw62gIP5WPAyL3KT9jcYuPHjRmOQx9eiO8h_8kjed7Bs8ijjSXUAr2RXIcZ/s1054/1.png)

3D Printing is a highly addictive hobby! This is the very first time I am using my 3D printer to print something electronics related. The STL files used in this project are all downloaded from www.Thingiverse.com. I have uploaded a copy of all the 3D Objects to my GitHub repository, the link is in the description below.

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhMgBkM2CvHgslQwVPNQzwgCo2YpTCOub1Qtkr-Y9K-UiLGiMTnHMbOGfdTW5rGl6ZdSsNwKmwI8p5teVT0ZOLOx-wkt26Yisnz5R6ZL0dbwFREflSDeg07nljRwA3u_3VmrB_JCQgDt6W4O7kjvGyQWvBFHcXJIJfVi5xVo30vNQjgt5SfEOatCf-6xNMt/s1054/2.png)

3D printing has changed my life. There are so many things you can do using a 3D printer. From designing 3D Models to printing them using the 3D printer has now become my new hobby. I've been a "maker" since I was 10 years old, and have always constructed and made my own stuff. 3D printing for me is a blessing. I am totally lost in the 3D printing heaven.

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhwNQrETD5JbqJbtRMpDXjnio30Rd0ZmpzV_cDL4ecLK_K6ryhnsZARhNAdjSnbSwWc9isykZQAThGRj_rxRJSIR9JZyX_Cqk3OmbE7FGPwvJgP2tQ5uapf6Q9qnxdhuhlPtXvmRnO-Ui7ajrqyIBYTcJ1pvphvtZowm3NS8sSz4gbSMeAIYyDQ7Cj9cLQI/s1054/4.png)

3D printing has changed my electronics workshop life forever. Before when I used to order parts, I always used to wonder if the parts would fit into my projects resources... but after I got my 3D printer... it doesn't matter at all, because if it doesn't fit - I could design and print it myself. The 3D printer was definitely "The Missing Piece" from my electronics workshop.


Schematic Diagram
-----------------
![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhQ_7vg2T6Im78OhSGpY_N_a760Sw0ParB4L196N4fqjAKmSMGhGSrTFxwyn62aJwWlexnheZcuvjVQIl5k7kiY3pWcLN-s7yHtXxr1Eg0Y7SvjY5aoqaHNuMcoAstO4PMFvDguoG-I-89SpaFxMvbgkfHEdzlDpdOBjlCLogd99yZ7Prz98OJ_rZd4RkPp/s1054/6.png)

Now that we have all our 3D Models printed, lets have a look at the component assembly.
The assembly is super simple. We just need to connect 4 Yellow LEDs to D2, D3, D4 and D5 pins of Arduino via 220ohm current limiting resistor.
Then connect the white LED to Analogue Pin D10 of the Arduino via a current limiting resistor.
That's it, as simple as that.


The Code
--------
![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjVRrexu1y3ggiRuKuyDwksS-PAcHzwdPbJ-NsUF5plGCn4wodx45qjVx8Xrpf0lRjAuZIx08hQV3ND2khN_BixCIpqXET0aUgEvhDad8kkDbkQ6tRrJzSeKIP19uPrazpITbMD5WimBq7wAmbOvncbhIPPC0IMz0emap59mLqyJViA56YvbeuX6yKGnRjW/s1054/7.png)

Now, lets have a look at the code that will drive the LEDs.
Lets start by defining all the variables. 
Then in the setup section lets define all the pin modes.

To flash the LEDs I chose 5 different Flashing patterns:
	1. All LEDs Flash Very Fast For 10 Seconds
	2. All LEDs Flash Slowly For 10 Seconds
	3. 2 LEDs Turn On and 2 LEDs Turn Off for 10 seconds 
	4. LED Chaser Circuit for 10 seconds
	5. One LED Randomly Turn On for 10 seconds
The switch statement in the loop() section randomly picks up one of these patterns and runs it for 10 seconds. 
The white LED also fades in and out after every cycle.

At the bottom of the code, I have defined all these 5 LED flashing patter in their respective functions.


Demo on BreadBoard
------------------
![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhF84VGpgbx5L6a9K5_nhHOpVym4uilsbZd5OzVsHn-4lt0MQLJXvSUhbl9LeNlfBRn-Ws3Fx3x-FmB5TFykWpp9BXHUHxdP3HoHWFZgfiriD4SDuj68WHcqh8Hu46X-hPkiupRlf4tTPD0rKu75-udmJ3-RwLYNWE0aLfE0u0r8WPFhE_n2JCRe9IBeB-P/s1054/8.png)

After loading the code on an Arduino Nano this is how it looks like.
The white LED will go inside the Ghost and the Yellow LEDs will go inside the Pumpkins.
Humm, that looks promising, isn't it?


Assembling 
----------
![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgerY7fiR-1dVWsPRGpoeZK_albQqUnSDbrIk9oGZK3D7Unvkr7r9ENrhYxaOoXfPorBOy44-D7LklTTFoA9vHTtniDQV6K31EafEB1hItvdpp3uWIVZFC_sV7Zti1GrWITQ0NeEbzMJkelty13hDrAb78-7KWpLufJxKbPum2KsTzgUmpFY8yL2dTGyAz-/s1054/9.png)

Let's start by soldering the wires to the LEDs.
Then lets solder the Arduino Nano to a perf-board and then solder all the resistors to the board.

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhhmtqraGbKPWM_SYiNprliJxbiskgpaUf4bm7O4TDbQC2BlLKcrlQwHAvZLF4yXxIoXD5L9iOWi5wBsTq1OTPegDDbfRAt_8xthhLvbrphaJXRUgCH5zv_dmg2AIYVQb8rEWDIdSkYkZbxfWfbfc4iBJOtBcPe1yXoaLwAgZaI322yh1rST367bThNYEyf/s1054/11.png)

Next, lets soldered the LEDs to the D2, D3, D4, D5 and D10 pins of the Arduino via the current limiting resistors.

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgNTKYXSAp7ZDB8XvOtHQIlOTc7axC4TuTj2Eoi08UEYWXVZ1401AWS3DSxZUJtIuOy5clYCz32HDnmlvcJ_fAkLThyphenhyphenQpbfof11ie1nGtwDRGw7-UZ8wICDWwM0kIuskhyphenhyphenT9Qs6FrpwY_6MtmqVWpbpWzLG0cV8fTELyF5ivIDbSeCVTNXNthlSec6vSxhR/s1054/12.png)

That's all you have to do for the electronics bit. Now, let's hot glue the perf-board inside the coffin, followed by all the LEDs to a wooden block.

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjk3ABPkd_JzQfq3BQ_ndfbAqhO9LdwfLwt8zkvyHqUsJCrJeEZhFZdXnr-QyLxx2VGAmZ6Lzp8DerskW4q1domEBVz9zcwj0oBUTj-nDq5Vor0glCuksE-EL1knvj6DwaZ37vIH1zWgICbmDgS-LhfGxTzmRXb79GloecIggwBDZv9-9dE3I5-ELBTx6HG/s1054/14.png)

Before putting the 3D printed components on the LEDs, let's do a quick test to verify everything works as expected. Look at that...

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgCFwGBf7wP_bWshO5VGq8TuTCG5cSG2hH99CpuVARRKJTRrdA1luoz0BU2eutNyPfxpsdrevlV_UJ-s6Bdm9cLzipGDlbzSKjnXrSMvLjrM0K8-MnkHF6Bvct4M0pdaMAMMwlI8dD1wpGxysvvtnfi4GEuZODeHBWwQV-SsbqMWk-l85pAo_FVYWP0aki0/s1054/15.png)

Now, one by one lets hot glue the 3D printed components to the plank. To finalize the setup, I added a few dry grass leaves to hide the wirings. That's it all done.


Final Demo
----------
![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhO5xgOfipaG7zS5WvodXwjeHxSWUUjGwA4y4-cLKewOYuHxV1lDAVwzTrTR5lbKu74SOr-UM7BHT3HZG34ZwmCNW9RK6dSKJjfPy78b6OdFnjOfPdT04fBzFkYISp7UyrI8-mdw9XuGktp9wWRBKbIE_rc6MQV0w613D8aHJCkKdL8UL_VzCmasAuKLGil/s1054/18.png)

So this is how my final setup looks like.
Do comment and let me know if there are any scopes of improvement. Until then, Happy Halloween....
 

Thanks
------
[![Hxfhwr0Eoqk](https://i.imgur.com/DDCVjuD.png)](https://youtu.be/Hxfhwr0Eoqk)

Thanks again for checking my post. I hope it helps you.
If you want to support me subscribe to my YouTube Channel: https://www.youtube.com/user/tarantula3

Video: https://youtu.be/Hxfhwr0Eoqk Visit 

Full Blog Post:  https://diy-projects4u.blogspot.com/2023/10/Halloween2023.html

Code: https://github.com/tarantula3/Arduino-Halloween--Decor/blob/main/Code.zip  

Schema: https://github.com/tarantula3/Arduino-Halloween--Decor/blob/main/Schema.fzz  



STL Files:
Coffin:  https://github.com/tarantula3/Arduino-Halloween--Decor/blob/main/Twist_Lock_Coffin.zip

RIP:  https://github.com/tarantula3/Arduino-Halloween--Decor/blob/main/RIP.zip

Pumpkins:  https://github.com/tarantula3/Arduino-Halloween--Decor/blob/main/Halloween_Pumpkins.zip

Pikachu:  https://www.thingiverse.com/thing:4701289

Ghost:  https://github.com/tarantula3/Arduino-Halloween--Decor/blob/main/Cute_Hug_Me_Ghost.zip

Instructables: https://www.instructables.com/3D-Printed-Arduino-Halloween-Décor/



**Support My Work:**

BTC:   1Hrr83W2zu2hmDcmYqZMhgPQ71oLj5b7v5

LTC:   LPh69qxUqaHKYuFPJVJsNQjpBHWK7hZ9TZ

DOGE:  DEU2Wz3TK95119HMNZv2kpU7PkWbGNs9K3

ETH:   0xD64fb51C74E0206cB6702aB922C765c68B97dCD4

BAT:   0x9D9E77cA360b53cD89cc01dC37A5314C0113FFc3

LBC:   bZ8ANEJFsd2MNFfpoxBhtFNPboh7PmD7M2

COS:   bnb136ns6lfw4zs5hg4n85vdthaad7hq5m4gtkgf23 Memo: 572187879

BNB:   0xD64fb51C74E0206cB6702aB922C765c68B97dCD4

MATIC: 0xD64fb51C74E0206cB6702aB922C765c68B97dCD4


Thanks, ca again in my next tutorial.



Cos: https://cos.tv/videos/play/47932030253831168

Odysee: https://odysee.com/@Arduino:7/3D-Printed-Arduino-Halloween-Decoration:d

Rumble: https://rumble.com/v3pg1if-3d-printed-arduino-halloween-decoration.html
