# 11056 Website
## _Reflection and Code for front end web design_

### Reflection

##### Thoughts On Visual Studio Code & GitHub Desktop
Upon reflection of this task I would like to firstly compare my past experience with the Glitch coding website to the applications used specifically the Visual Studio Code & GitHub Desktop applications.

In being completely honest initially I was concerned in having to learn two new programs as I could only imagine the clash between the techniques I developed during my brief use of glitch and the ones required for the Visual Code app. To my surprise and what I would consider a motivational benefit the to me the two programs as I call them worked in general, the same. The only main differences I noticed were on the two methods in which you can check the website on the web and interactions such as moving files and or images though I found these didn’t take long to get used to and I wouldn’t say I prefer one over the other I would just describe them as different, but on another hand… **One auto saves, has a auto format button and gives you a simple link to view your project on any device!!!** And the other, does not, something I found to be quite annoying ‘o’ did I mention that Visual Code basically relies on Github to publish your work online not impressed with that either, seems like an after thought. Though in hindsight I can defiantly say I am as a result much quicker on a keyboard due to the constant saving, tabbing swiping and quick google searches, in a quick brake from knocking Visual Code I did find the colour contrast between the text, tags and etc were better than those on Glitch and I will always having my work on my laptop auto updating to iCloud certainly brought its comforts and reassurances.

#### Website & Code

Starting with the website I found that, for lack of better words, this work slowly grew into itself as by using my low fidelity prototypes and my initial code I quickly had a scaffolding of what the website was doing too look like. With of course plenty of alteration along the way I feel far happier with the quality and appearance of the website than the one I have previously built using Glitch. Now that its as complete as it can be in its time frame and my limited skill set with coding there are a few things I would like to note;

**Colours:** In terms of colour I am especially happy with the blue and grey highlights any of the interaction ‘buttons’ have I feel that it makes them, like many websites that use the same technique more noticeable and brings a sense of interaction. I Also am happy with how I was able to show which page was active by permanently highlighting it blue ( if we are going to be specific then, #6cb6f3 ) and to my surprise it wasn’t as hard as I originally thought. To finish this section I am again happy with the tone of blue I chose as I believe it resembles a ‘Canberra blue’ although I believe I could further enhance the appearance of the website quite easily by adjusting the shades of greys that I used and by swapping my red footer to the same Canberra blue. 


**Fonts:** Essentially with in terms of fonts I went with the classic and clean looking times new roman and its similar back up fonts, as I believe it again fitted the Canberra theme which I believe is important as the website is promoting a Canberra based event/s.

**Layout:** In terms of the layout the reason I chose the layout I did as I believed it kept the website mostly clutter free and this is especially science in the Events, Artists & Works and Our Team categories through the use of cards and columns, and in reflection I believe that this layout does in fact achieve that, although it needs some minor formatting modifications such as the positions of the titles in the cards and there backgrounds, and lastly be able to make all the cards the same size and have a link so you can view more, as I sadly I wasn’t able to figure out how to do that for this assignment.

**Interactive:** By far the hardest element of building the website was trying to make it interactive I will complete admit I though it was going to be easy as, and as a result give full credit to the people who manage to do it well, as I ran into issue after issue especially with the header and the information cards and grid layouts.

#### Code

Finally as I conclude below I will display of some of the issues I came across / elements I just couldn’t get work, and ended up having to re- code them in an entirely different way. Below shows one of attempts at  adjusting the search bar using CSS, which was forfeited after I wasn’t able to make it line up with the rest of the header and especially when the screen size changed.
```
<div class="searchbar">
<input type="text" placeholder="Search..">
</div>
</div>
</div>


  /* Add a black background color to search bar*/ 
.searchbar {
    overflow:visible;
    background-color:none;
    margin-top: 1%;
    margin-bottom: none;
   float:left;

  }
 /* Change the color of links on hover */
  .searchbar a:hover {
    background-color: #ddd;
    color: black;
    width: 100%;
    height: auto;
  }
  
  /* Style the "active" element to highlight when in use or on page */
  .searchbar a.active {
    background-color: #2196F3;
    color: white;
    width: 100%;
    height: auto;
  }
  
  /* Style the search box inside the navigation bar */
  .searchbar input[type=text] {
    float: right;
    padding: 4% 2%;
    border: none;
    margin-top: 1%;
    margin-right: 0%;
    font-size: 12pt;
    width: 100%;
    height: auto;
    
  }
 /* Style the links inside the search bar */
  .searchbar a {
    float: right;
    display: block;
    color: black;
    text-align: center;
    padding: 2% 2%;
    text-decoration: none;
    font-size: 17pt;
    width: 25%;
    height: auto;
    
  }
  ```
Below shows the final code I used and which solved the issues caused by the code above whilst also allowing me to customise the characteristics of not only the search bar but also the header to a far greater extent and more easily.
```
/* Add a black background color to the top navigation bar */
.topnav {
    overflow: hidden;
    background-color: #e9e9e9;
    width: 100%;
    height: auto;
 
  }
  
  /* Style the links inside the navigation bar */
  .topnav a {
    float: left;
    display: block;
    color: black;
    text-align: center;
    padding: 5px 0;
    text-decoration: none;
    font-size: 17pt;
    width: 15%;
    height: auto;

  }
  
 
    /* Change the color of links on hover */
    .topnav a:hover {
        background-color: #ddd;
        color: black;
        width: 15%;
        height: auto;
      
    }
      /* Style the "active" element to highlight the current page */
      .topnav a.active {
        background-color: #6cb6f3;
        color: white;
        width: 15%;
        height: auto;
      }
  /* Style the search box inside the navigation bar */
  .topnav input[type=text] {
    float: right;
    display: block;
      text-align: center;
      width: 15%;
      margin-top: 0%;
      margin-bottom: 0%;
      padding: 10px;
      height: auto;
      margin-left: 5%; 
      margin-right: 3%;
  }
  
  /* When the screen is less than 600px wide, stack the links and the search field vertically instead of horizontally */
  @media screen and (max-width: 600px) {
    .topnav a,.topnav input[type=text]  {
      float:center;
      display: block;
      text-align: center;
      width: 33.33%;
      margin-top: 15px;
      padding: 15px;
      height: auto;
      margin-left: 30%; 
      margin-right: 33%;
    }
```


Sadly my troubles didn’t end here as again ( two old attempts ) shown below I Had various attempts at coding in an interactive and linked button/s into the header though the code below did work it didn’t work very well and I wasn’t able to make it responsive to different screen sizes.

```
<div class="header-centre">
<a href="Events.html">  <button class=" button">Events</button></a>
<a href="Artists.html"> <button class=" button">Artists & Works</button></a>
<a href="ourteam.html"> <button class=" button">Our Team</button></a>
```
And
```
div class="header">
<a class="active" href="contactus.html"></a>
<a href="index.html" class="buttonlogo">  
<img src=“https://images.squarespace-cdn.com/content/v1/5e142229c73726304407e983/d63ab98b-162e-4fbc-a917-a8423ab55bd8/CAB%2Bc556+606+656.png?format=1500w"
/></a>

.buttonart {
    border: none;
    outline: 0;
    display: inline-block;
    padding: 8px;
    color: white;
    background-color: #000;
    text-align: center;
    cursor: pointer;
    width: 100%;
  }
```

To breifly conclude my reflection though I was initially hesitant to use the platforms which were used to build this website, after experiencing them I now understand as to why they are used professionally in replacement of a another platform such as Glitch and I believe that though I am currently restricted with my limited coding skill set with some minor tweaks such as the ones previously mentioned I would be able to greatly improve this website and even more so with more experience and time.