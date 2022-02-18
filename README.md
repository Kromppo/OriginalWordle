# Original Wordle Resurrection 
Isn't it funny that the NYT paid seven figures for a website you can use offline?

The original game was created by [Josh Wardle](https://twitter.com/powerlanguish) 

**[The Verge: New York Times acquires Wordle](https://www.theverge.com/2022/1/31/22911274/wordle-new-york-times-free-word-game-acquisition)**

**[Wayback Machine of the Original Version](https://web.archive.org/web/20220210031511id_/https://www.powerlanguage.co.uk/wordle/)**

Since the official game is now hosted on the NYT website, they will most likely paywall
it in the near future. They already edited the word list on 2/15/21 so it no longer 
matches the original. Here is a guide on how to download the original website and play
offline since all the code is client-side and baked into it locally. This guide also 
details how to import your statistics from the official website, along with links to
Wordle alternatives in case you can't wait 24 hours for the next word. Lastly, don't feel
too bad about that 6/6. Visit https://twitter.com/wordlestats to see how many other players 
don't have a strong command of the English language. 

## Saving the Website Offline

Unless you are looking for a specific file, download the [Latest Release](https://github.com/Kromppo/OriginalWordle/releases/tag/Latest) and then continue with the guide, skipping over any steps requiring a download. The latest release will have all needed files. If you experience any issues, check [Issues](https://github.com/Kromppo/OriginalWordle/issues) to see if the bug is known, or if a fix has been implemented already. If not, open a new one (for duplicates just comment on the existing one). Do not use this section for enhancement suggestions. Use the [Discussions](https://github.com/Kromppo/OriginalWordle/discussions) tab instead!

### Downloading Wordle 
 >Windows/macOS
 1. Download [Wordle.zip](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/Kromppo/OriginalWordle/blob/main/Wordle.zip)
 2. Extract the .zip to any directory on your PC 
 3. Extract again until you have the base folder called Wordle
 4. Double click **Wordle.html** to open in your default browser
 
### Alternative Method (Web Archive)
>Windows/macOS
 1. Go to [Wordle Wayback Archive](https://web.archive.org/web/20220210031511id_/https://www.powerlanguage.co.uk/wordle/)
 2. Play the game as you normally would or continue to Step 3 for offline use.
 3. Save the page as a .html (Right Click > Save As...)
 4. **Make sure it is saved as Webpage Complete**
 5. If you are part of the few that haven't figured out how to use dark mode, you can open <br /> the .html  and play from here. Otherwise, follow the steps below to come to the dark side. 
 6. Open up **Wordle.html** in any text editor and scroll all the way to the bottom of it
 7. Find the line where it says `<body class="nightmode">` and change it to just `<body>`

### Playing on Android
 > This section assumes you know the basics of USB Debugging and PC File Transfer
 1. Connect your device to a PC via USB and click allow on the popup
 2. Change the USB Preference to File Transfer
 3. Open the PC file explorer and navigate to your phone's internal storage
 4. Go to `Android\data\com.brave.browser\files\Download\` or the same path for your default browser
 5. Paste the Wordle.zip and extract it into this directory
 6. Open the browser search bar on your phone and enter `file:///sdcard/AndroidAndroid/data/com.brave.browser/files/Download/Wordle/Wordle.html`
 7. Bookmark this page for ease of access.
 8. If you have any issues follow this [reddit guide](https://www.reddit.com/r/wordle/comments/sijwvn/anyone_know_if_a_good_android_app_that_can/hvgkasl/?utm_source=share&utm_medium=web2x&context=3)

### Playing on iOS
> Maybe it's time to escape the walled garden
 1. Go to [Wordle Wayback Archive](https://web.archive.org/web/20220210031511id_/https://www.powerlanguage.co.uk/wordle/)
 2. Either you can play from here normally or save the website offline as a [Web Archive](https://support.apple.com/guide/safari/save-part-or-all-of-a-webpage-ibrw1089/mac)
 3. Effectiveness of this method is unknown but it is a workaround unless someone finds the iOS version of the method above

# Importing Your Statistics
  1. Download [sethistory.html](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/Kromppo/OriginalWordle/blob/main/sethistory.html) and place it in the same directory as **Wordle.html**
     > DO NOT put it in Wordle_files. Keep it on the same level as the other HTML <br />
     > Extract the .zip until you have the base HTML file
  2. Open up **sethistory.html** in any text editor and pull up your old statistics
  3. Follow [this guide](https://leancrew.com/all-this/2022/02/resurrecting-the-old-wordle-for-procrastinators/) to input your statistics 
  4. Lines 38-45 were purposefully deleted. Don't replace them
     > Setting game state values locked the website to that day when you imported statistics
  5. Double click sethistory.html and then click on the _**Set History**_ Button
  6. On Android, follow the same steps as the Wordle HTML for accessing this file
  7. If you want to do it entirely manually follow [this guide](https://nerdschalk.com/did-wordle-streak-reset-for-you-heres-why-and-how-to-get-it-back/)
     > The sethistory file imports all data but current streak. Use this to fix current streak

# Alternative Versions
>Considering the infinite pop-up of wordle clones, not every version will be linked here or in the wayback archive. 
>Only the most intriguing takes on the game will be linked. Check [Discussions](https://github.com/Kromppo/OriginalWordle/discussions) for links to other verisions, or open a new thread if the version doesn't have one yet (Check FIRST!)

[Absurdle](https://qntm.org/files/absurdle/absurdle.html)
| The adversarial version of wordle, you are trying to box in the bot as fast as you can using your guesses so the options to pick are only limited to one word. Every time you guess, it picks a new word from the largest group of possible options given the current colors of all the guessed letters. The minimum number of guesses to win this game is 4. It's recommended to read the entire tutorial before starting this game. This game has unlimited daily plays and unlimited guesses. 

[Nerdle](https://nerdlegame.com/)
| The math fanatics version of wordle: Instead of words, you are trying to solve an equation. Just like wordle guesses have to be a valid word, guesses have to be valid equations. The game resets at midnight local time and you have six guesses. 

[Worldle](https://worldle.teuteuf.fr/)
| The geographical version of wordle: You are trying to guess the country based on its shape. Every guess tells you your proximity and direction of the correct country based on the country you guessed. It resets once a day at midnight local time and you get six guesses.

[Globle](https://globle-game.com/)
| Also a geographical version but visual. Instead of telling you the proximity to the country, it colors the country redder the closer you are, and yellower the farther you are. The game also tells you your closest guess so far. There is one game a day but you have an infinite number of guesses. 

[Dordle](https://zaratustra.itch.io/dordle)
| The double version of wordle: You are playing two wordles at once, but with the same set of guesses. This game has the daily version and the infinite play version.

[Archive](https://metzger.media/games/wordle-archive/)
| The retrospective version of wordle: If you missed a day, or want to replay previous days, you can pick from the list. It pulls from the NYT word list so it will not match the original version of games after February 15, 2021. 

[Unlimited](https://wordlegame.org/)
| If your wordle craze hasn't worn off and you didn't realize the bubble is bursting, this is wordle but with unlimited play plays. It is played just like the original game. 

# Other Relevant Links

[3Blues1Brown Part 1](https://www.youtube.com/watch?v=v68zYyaEmEA&ab_channel=3Blue1Brown) Solving Wordle using Information Theory

[3Blues1Brown Part 2](https://www.youtube.com/watch?v=fRed0Xmc2Wg&ab_channel=3Blue1Brown) Oh, wait, actually the best Wordle opener is not “crane”…

[WVFRM Podcast](https://www.youtube.com/watch?v=X_e2IEaR4aA&ab_channel=WVFRMPodcast) The origin story of the project and Josh's previous work

[No Markup Version of ReadMe](https://pastebin.com/ip48vYZG) The RAW Text version in the event something breaks 

[Wayback Archive links](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/Kromppo/OriginalWordle/blob/main/WebArchiveList.txt) A text document of all the links mentioned in the guide

`Updated 2/18/2022`
