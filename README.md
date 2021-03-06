# DrFrostMaths
A resource on [DrFrostMaths](https://www.drfrostmaths.com/) exploits.

## How to set up the bot
Requirements:

• [Node](https://nodejs.org/en/download/) (latest version)

### Getting the required cookies
Firstly, you will need to get your [_ga](https://i.imgur.com/KAHd7Kl.png) cookie and your [PHPSESSID](https://i.imgur.com/kg7gV1C.png). You can get it by getting the extension called [EditThisCookie](https://chrome.google.com/webstore/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg?hl=en).

After you have gotten the two cookies, paste them in the [config.json](https://github.com/Stefanuk12/DrFrostMaths/blob/main/Bot/config.json) file, which should now look like [this](https://i.imgur.com/R4Mboxb.png)

### Getting the correct aaid
After you've gotten the cookies, you will need to get the aaid. You can getting it by going to this [link](https://www.drfrostmaths.com/keyskills.php?tid=1&permid=196) then pressing **Start Practice**, make **Completion** as **Keep going until I say**, and press **OK**.

If the link doesn't work, the question you need is called `#9: Adding integers with a written method.`

After you've done that, look at the URL, it should look something like: `https://www.drfrostmaths.com/do-question.php?aaid=15326547`. You want to get the aaid at the end, so the aaid would be **15326547**.

Great, you've gotten the aaid, now paste it near the end of [index.js](https://github.com/Stefanuk12/DrFrostMaths/blob/main/Bot/index.js#L131) where it says `AAIDHERE`, it should now look like [this](https://i.imgur.com/68ZB8JW.png)

### Launching the bot
After doing all of the above, you will need to open a terminal/command prompt in the installation directory and type the following commands:

This command will install of the required dependencies
```bash
npm i
```

This command will run the bot
```bash
node index.js
```

# How to skip videos
You want to copy the code in [index.js](https://github.com/Stefanuk12/DrFrostMaths/blob/main/Skipping%20Videos/index.js) then open up Inspect Element. After opening up Inspect Element, navigate to the console, paste the code, and run it. Now, watch the video and after a few minutes, it will register the video as finished. If I find a better way of doing it, I will update the script.
