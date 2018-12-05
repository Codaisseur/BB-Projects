# Developer Tools: Git & GitHub

## 🎨 What we will build
In this part we will set you up to use two of the most important tools of the Developer tool box: Git & GitHub


## 🎯 Learning Goals
By the end of this section, you will learn:

* [ ] how to navigate and do basic management of the file system from the shell
* [ ] how to use git & gitHub for version tracking


## 📚 Modules that will be discussed

* [Terminal 1]()
* [Terminal 2]()
* [Git 1]()
* [Git 2]()

## ✏️ Assignments

### Create a directory

1. Open your terminal and create a new directory called codaisseur. Don't forget to hit enter!
![mkdir codaisseur](https://cd.sseu.re/1._mimiCodaisseursMBP2__zsh_2018-11-28_15-30-35.png)

>  _❗️ Your terminal might look somewhat different and have different colors, that is ok!_ 

2. Change directory into your new folder codaisseur:
![cd codaisseur](https://cd.sseu.re/1._mimiCodaisseursMBP2_codaisseur_zsh_2018-11-28_16-04-30.png)


> ## 👌 Pro-tip
> _Use tab completion to show your options: start typing the name of your directory and hit tab. In my case, I have a `Code` and a `codaisseur` folder in my home directory In your case, the terminal might simply complete the word you were typing._
>
> ![Tab completion](https://cd.sseu.re/1._mimiCodaisseursMBP2__zsh_2018-11-28_15-40-02.png)

3. Now, create a a new directory called `week-1` with the command `mdkir week-1` and change directories into `week-1` by running `cd museum-app`. Use the command that displays your current working directory (`pwd`) to check where you are:

![pwd](https://cd.sseu.re/1._mimiCodaisseursMBP2_codaisseurweek-1_zsh_2018-11-28_16-09-37.png)

4. Finally, create a new directory called `museum-app` and change directories into it. When you use the command that displays your current working directory, you should see something like: `/Users/[YOUR NAME]/codaisseur/week-1/museum-app`.

That's it! You are all set up!

### Initialize a git repository and commit your first change

Next up, we will initialize a git repository (repo) to keep track of all your changes. You'll be creating a new git repo for every new project during the academy and beyond...

1. Check whether you are in your project directory:
![Check working directory](https://cd.sseu.re/1._mimiCodaisseursMBP2_codaisseurweek-1museum-app_zsh_2018-11-28_16-17-21.png)

2. Run `git init` to initialize a new git repository
![git init](https://cd.sseu.re/1._mimiCodaisseursMBP2_codaisseurweek-1museum-app_zsh_2018-11-28_16-19-47.png)

3. Open your project in Visual Studio Code by running `code .` Your computer should open this window:
![VSC](https://cd.sseu.re/Welcome__museum-app_2018-11-28_16-22-17.png)

4. Click on the side bar of VSC and type `a` (or right click on it and select `create file`). After that, type the name and extension of your file. In our case, that is `README.md`.
![create new file](https://cd.sseu.re/Welcome__museum-app_2018-11-28_16-31-13.png)
![name new file](https://cd.sseu.re/Welcome__museum-app_2018-11-28_16-28-09.png)

5. Copy the following text in your `README.md` and safe the file (`cmd + s` or `ctrl + s`):

```
# Museum App
```

> ## 👌 Pro-tip
> Especially in the beginning, your code will often not work because you forgot to safe it. If you see this circle in the tab of your VSC, it means you did not safe that page yet!
>
> ![not safe sign](https://cd.sseu.re/README.md__museum-app_2018-11-28_16-37-24.png)

6. Use `cmd tab` or `ctrl tab` to switch screens to your terminal. In there, use `gst` to check whether git registered your changes:
![gst](https://cd.sseu.re/1._mimiCodaisseursMBP2_codaisseurweek-1museum-app_zsh_2018-11-28_16-43-40.png)

7. Use the command `git add .` to select all your changes for the next commit. Check whether they are staged by running `gst` again:
![gst stage](https://cd.sseu.re/1._mimiCodaisseursMBP2_codaisseurweek-1museum-app_zsh_2018-11-28_16-46-17.png)

8. Now commit your change with the command `git commit -m 'Add readme'`. Check whether it worked by running `gst`

![gst commit](https://cd.sseu.re/1._mimiCodaisseursMBP2_codaisseurweek-1museum-app_zsh_2018-11-28_16-48-51.png)

### Push your changes to github
With a git repository we can track our progress, however, it runs only on our local machine. So let's make sure we can store (and present) our project online!

1. Go to [www.github.com](https://github.com/). After logging in, click on the plus icon and choose `New Repository`:
![new repo on GitHub](https://cd.sseu.re/GitHub_2018-11-28_16-50-59.png)

2. Create a new repository: 
![create new repo](https://cd.sseu.re/Create_a_New_Repository_2018-11-28_16-54-25.png)

3. You will be redirected to a new page. Copy the following lines in your terminal:

![push existing repo from command line](https://cd.sseu.re/MimiMagmusum-app_2018-11-28_16-58-07.png)

4. If all is well, your terminal window will look something like this: 
![terminal window](https://cd.sseu.re/1._mimiCodaisseursMBP2_codaisseurweek-1museum-app_zsh_2018-11-28_17-00-33.png)

5. If you refresh your page on GitHub, it should look like this:
![succes GitHub](https://cd.sseu.re/MimiMagmusum-app_2018-11-28_17-02-13.png)

Well done! You set up a repository on GitHub, added the (remote repository) to git and pushed your first changes to GitHub!

## 🎯 Learning Goal Tracker
In this section, you learned...

* [X] how to navigate and do basic management of the file system from the shell
* [X] how to use git & gitHub for version tracking
* [ ] how to use Chrome DevTools to inspect the HTML of a page
* [ ] how to create an HTML page in your text editor and open it in the browser
* [ ] some important HTML tags, and when/why you should use them.
