# numb3r
A script that translates a number to a list of words acording to a letter-to-number mapping.

The idea of this script is to help generate large sequences of words/objects that you can easily memorize (using techniques like the mind palace, etc).
It assumes that you have a letter-to-number mapping. Take the following:

| Derren | Brown's | Mapping |
|:---:|:---:|:---:|
| 's' -> '0' | 'r' -> '4' | 't' -> '7' |
| 'z' -> '0' | 'f' -> '5' | 'ch' -> '8' |
| 'l' -> '1' | 'v' -> '5' | 'sh' -> '8' |
| 'n' -> '2' | 'b' -> '6' | 'j' -> '8' |
| 'm' -> '3' | 'p' -> '6' | 'g' -> '9' |


If you were presented with the number **454**, using the map above you could translate it to **RVR** which in turn could be represented by the word **RiVeR**.
  
If you had a bigger number like **454433902** then you might not find a single word that you could translate to. However a possible solution could be to use multiple words like **RiVeR aRMy MaGaZiNe**. This notebook tries to find those words for you. For example, if you were to memorize Pi up to 100 digits you could use the script to get a list of words that would best match its digits.
  
The script uses a list of concrete nouns so that the used words are easily memorized plus it takes into account the frequency of that word in the whole of wikipedia so that the most popular words are picked instead of just the longest.

As mentioned, also included in this repo are two files with a set of concrete nouns for both Portuguese and English:

**en/nounlist_frequency.csv**  
**pt/nounlist_frequency.csv**  

These lists need further improvement so please feel to contribute.
