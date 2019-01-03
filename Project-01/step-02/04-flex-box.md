# Positioning & Responsive Web Development

## 🎨 What we will build
In this section, you will finish the styling of your index page. The end result will look something like this
**TODO!!!!!!**


## 🎯 Learning Goals
By the end of this section, you will learn:

* [X] how to apply some of basic concepts of responsive web development


## 📚 Modules that will be discussed

* [CSS 3]()


## ✏️ Assignments
#### Make it work for mobile
When you compare the app you created so far to the example app, we see a couple of differences:
![spacing differences](https://cd.sseu.re/MuseumGuide_2018-12-11_09-20-33.png)
Since we are trying to rebuild the example app, we'll have to work on how we position our images in our gallery. We'll try to make it look good on your phone first, after, we'll make it work on our desktop.

1. Change your view to mobile:
![mobile view DevTools](https://cd.sseu.re/Museum_Guide_2018-12-11_09-29-32.png)
2. Inspect the first image and copy the styles to your `index.css`. Answer the following questions:
    * What happens if you change `.artObject` to `artObject`? Why does that happen?
    * What happens if you replace `max-width` with `width`?
    * What happens if you replace `max-height` with `height`?
3. Change your view to different types of mobile devices and check whether your page still looks ok (it should, I just want you to switch views 😉): ![switch mobile device](https://cd.sseu.re/Museum_Guide_2018-12-11_09-37-48.png)

> ## 👌 Pro-tip
> If you copy code, make sure your indentation is still correct!

#### Gallery title
When the screen is big enough, the title 'Gallery' should be placed next to the images. In mobile view, it should be above.

1. Change your view back to normal: ![mobile view DevTools](https://cd.sseu.re/Museum_Guide_2018-12-11_09-29-32.png)
2. In the example app, inspect the `<section>` with the id `gallery`. Which code is responsible for placing items horizontally or vertically?
3. Copy the styles for `#gallery` to your `index.css`. What happens if you change...
    * ... the value of the `flex-flow` property to `column`? 
    * ... the value of the `align-items` property to `flex-end`?

#### Push your changes to GitHub
Check your changes, select the ones you want to commit, commit and push them to your branch.

 ```shell
 $ gst 
 $ git add .
 $ git commit -m 'Style gallery'
 $ ggpush
 ```

#### Merge into master
We build our feature! Let's merge everything into master.

1. Checkout your GitHub repository page and click the green button:
![Create PR](https://cd.sseu.re/Monosnap_2018-11-29_17-14-47.png)
2. Add a description and press the green button again:
![Add description](https://cd.sseu.re/Comparing_master...featindex-page__MimiMagmuseum-app_2018-11-29_17-37-49.png)
3. If there are no merging conflicts, press the button `merge pull request`:
![Merge PR](https://cd.sseu.re/Featstructure-index-page_by_MimiMag__Pull_Request_1__MimiMagmuseum-app_2018-11-29_17-39-19.png)
4. Click confirm merge:
![Confirm Merge](https://cd.sseu.re/Featstructure-index-page_by_MimiMag__Pull_Request_1__MimiMagmuseum-app_2018-11-29_17-40-28.png)

5. In your terminal, in `museum-app` checkout the master branch and pull the latest version from origin:
```shell
$ git checkout master
$ ggpull
```

## 🎯 Learning Goal Tracker
In this section, you learned...

* [X] how to use Chrome DevTools to inspect the CSS of a page using different views
* [X] how to create an CSS page in your text editor and link it to your HTML file
* [X] how to style specific elements on a page
* [X] how to apply some of basic concepts of responsive web development
