# We Keep Secret Drafts

A mysterious organisation has found a way to communicate with each other by hiding messages on a popular website. We have found this audio file which is apparently a song from a movie. Can you find out the secret message?



## Finding the song name

On listening to the audio file, we can hear a **reversed song** on one side and some noise on the other. Hence let us open this up on audacity and try to reverse the song. We can split the track into mono and then remove the noise part and then reverse it. On doing so we can hear a sped up song. So let us decrease the speed. On doing so we can understand the lyrics more clearly. On googling the chorus, we find the song is called **Spies like us by Paul McCartney**. 
![](https://dl.dropboxusercontent.com/s/00v4q49hqkpk7ea/songname.png?dl=0)


## Finding the flag
Let us check the **metadata** of the file to get more clues. ![](https://dl.dropboxusercontent.com/s/tmjgnw6r46a01ia/metadat5.png?dl=0)
We get a lot of hints from the metadata. We can see the mention of online encylcopedia which is obviously Wikipedia, another hint is the name of the challenge We keep sounds like wiki. There is also a base64 text to rot13 encoded text, which translates to **draft**. Other hints relating drafts are the name of the challenge and the name of the file. On googling wikipedia draft we get a hint that the flag is probably in the wiki drafts page of the song/movie.
On going to  
https://en.wikipedia.org/wiki/Draft:Spies_Like_Us
we find that it says doesnt exist/deleted.
![](https://dl.dropboxusercontent.com/s/6tqsb2gr0z586ak/wikidraft.png?dl=0)

Hence lets check it on the wayback machine. 
https://web.archive.org/web/20210805145506/https://en.wikipedia.org/wiki/Draft:Spies_Like_Us
We get the flag.
 ![enter image description here](https://dl.dropboxusercontent.com/s/rsfxvfmsd0t2a75/wiki2021-10-10%20200319.png?dl=0)