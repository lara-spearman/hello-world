## The trial page 

You can use the [editor on GitHub](https://github.com/lara-spearman/hello-world/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
Members should appear here
 
{{ page.title }}
 
{% if page.title %}
 Show {{ page.title }}
{% endif %}
    
{% assign course1 = site.data.courses.course | where "course", "A" %}


{% if site.data.courses %}
<ul>
 <li>
  <details>
   <summary> 
 Course 1: {{ site.data.courses.course =="A" }}
     {{ site.data.courses[1].rating }}
   </summary>
  </details>
 </li>
 <li>
 Course 2: {{ site.data.courses[1].course }}
 </li>
</ul>
{% endif %}


#This should appear as a dropdown
<details>
            <summary> This should reveal a list </summary>
            
            1. Course list 
            2. rating of course
            
</details>

{{ site.data.courses.course }}

### Contents of this page 
1. Trial review page
2. Trial text 

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3
print(5/6)
- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

```

```
### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/lara-spearman/hello-world/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

<!doctype html>
<html lang="en-US">
        <!--The code is messy, so feel free to modify it using better techniques and practices.-->

<head>
    <link href="https://fonts.googleapis.com/css?family=Playfair+Display" rel="stylesheet">

    <style>
        * {
            font-family: "Playfair Display"
        }

        h1 {
            color: blue;
            font-size: 48;
        }

        p {
            color: red;
        }

        div {
            background-color: white
        }

        #1 {
            background-color: #aacbff;
        }

        .row {
            font-size: 21px;
        }

        #circle_text {
            display: inline-block;
            padding-left: 10px;
        }

        p {
            color: black;
        }

        #circle1 {
            width: 30px;
            height: 30px;
            background: red;
            -moz-border-radius: 50px;
            -webkit-border-radius: 20px;
            border-radius: 200px;
            border: 1px solid red;
            display: inline-block;
            padding: 0px;
            font-family: "Playfair Display":
        }

        #singleline {
            display: inline-block;
        }

        #circle2 {
            width: 30px;
            height: 30px;
            background: #328314;
            -moz-border-radius: 50px;
            -webkit-border-radius: 50px;
            border-radius: 200px;
            border: 1px solid #328314;
            display: inline-block;
            padding: 1px;
        }

        #circle3 {
            width: 30px;
            height: 30px;
            background: #0089ff;
            -moz-border-radius: 50px;
            -webkit-border-radius: 50px;
            border-radius: 200px;
            border: 1px solid #0089ff;
            display: inline-block;
            padding: 1px;
        }

        textarea {
            resize: none;
            border-radius: 7px;
            border: solid 2px #78a1cb;
            /*white-space: nowrap;*/
            font-size: 17px;
            height: 31px;
            padding-left: 4px;
            padding-right: 1px;
            width: 100%;
        }

        #game {
            padding-left: 6px;
            padding-right: 3px;
        }

        .buttonRed {
            background-color: red;
            /* Red*/
            border: none;
            color: white;
            padding: 8px 18px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            font-weight: bold;
            margin: 4px 2px;
            cursor: pointer;
            border-radius: 5px;
        }

        .buttonRed:hover {
            background-color: rgba(255, 115, 0, 0.767)
        }

        .buttonBlue {
            background-color: rgb(0, 0, 255);
            border: none;
            color: white;
            padding: 8px 18px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            font-weight: bold;
            margin: 4px 2px;
            cursor: pointer;
            border-radius: 5px;
        }

        .buttonBlue:hover {
            background-color: rgba(38, 0, 255, 0.623)
        }

        /* Create four equal columns that floats next to each other */

        * {
            box-sizing: border-box;
        }

        /* Create four equal columns that floats next to each other */


        #t1 {
            margin-top: 50px;
            text-align: left;
        }

        .type {
            text-align: center;
            color: #756bea;
            font-size: 29px;
        }

        /* Responsive layout into 2 col - makes a two column-layout instead of four columns */
        @media screen and (max-width: 900px) {
            .column25 {
                width: 50%;
            }

            .column50 {
                width: 50%;
            }

            .column33 {
                width: 100%;
            }

            .column67 {
                width: 100%;
            }
        }

        /* Responsive layout into 1 Col - makes the two columns stack on top of each other instead of next to each other */
        @media screen and (max-width: 600px) {
            .column25 {
                width: 100%;
            }

            .column50 {
                width: 100%;
            }

            .column33 {
                width: 100%;
            }

            .column67 {
                width: 100%;
            }
        }

        #other {
            text-align: center;
        }


        .ml00 {
            margin-left: 0px;
        }

        .ml10 {
            margin-left: 10px;
        }

        .ml30 {
            margin-left: 30px;
        }

        .ml50 {
            margin-left: 50px;
        }

        .ml75 {
            margin-left: 75px;
        }

        .ml90 {
            margin-left: 90px;
        }

        .ml100 {
            margin-left: 100px;
        }

        .cType {
            color: black;
        }

        .rButton {
            margin-left: 15px;
        }

        /*#c1,c2{
        
    }
    
    .clear{
        clear: both;
    }*/

        .Alldiv {
            text-align: center;
            font-size: 21px;
            float: left;
        }

        .mealType {
            text-align: left;
        }

        .box {
            color: black;
            padding: 5px;
            margin: 10px;
            border-style: groove;
        }

        .grid {
            text-align: center;
            font-size: 20px;
            margin: 1px;
            float: left;
        }

        .top2 {
            margin-top: 12px;
        }

        .right2 {
            margin-left: 26px;
        }

        .extra1 {
            margin-top: 16px;
        }

        .extra2 {
            margin-top: 16px;
        }

        .cuisine {
            margin-top: -12px;
        }
        }

        .input-hidden {
            position: absolute;
            left: -9999px;
        }

        input[type=radio]:checked+label>img {
            border: 1px solid #fff;
            box-shadow: 0 0 3px 3px #090;
        }

        /* Stuff after this is only to make things more pretty */
        input[type=radio]+label>img {
            width: 20px;
            height: 20px;
            transition: 500ms all;
        }

        input[type=radio]:checked+label>img {
            transform:
                rotateZ(-10deg) rotateX(10deg);
        }

        #divleft {
            float: left;
        }

        #divright {
            float: right;
        }

        #cardioType {
            float: left;
            width: 100%;
        }

        .check {
            margin-top: 20px;
            margin-right: 10px;
        }

        .check2 {
            margin-top: 5px;
            margin-left: 10px;
            margin-right: 13px;
        }

        .check3 {
            margin-top: 20px;
            margin-right: 23px;
        }

        .check4 {
            margin-top: 5px;
            margin-left: 10px;
            margin-right: 9px;
        }
    </style>

    <title>Feedback</title>
</head>

<body>

    <div style="align-content: center; align-self: center;">
        <h1 style="align-content: center; align-self: center; align-self: center;text-align: center;">
            <u>Feedback Page</u></h1>
    </div>

    <p style="text-align: center; margin-top: -10px; font-size: 17px;">Feedback Message</p>


    <div style="width:10%; float:left;">
        <br>
    </div>
    <div style="width:50%; float:left;">
        <p style="text-align: center;">Question 1?</p>
        <p style="text-align: center;">Question 2?</p>
    </div>
    <div style="width:20%; float: left;">
        <div style="width: 100%; margin-top: 10px;">
            <input style="align-content: center; text-align: center; align-content: center;" type="radio" class="1 input-hidden" id="ar112" name="q1" />
            <label for="ar1"><img style="width:10; height:10;" src="red2.png" alt="No"></label>
            <input type="radio" class="1 input-hidden" id="ar2" name="q1" checked />
            <label for="ar2"><img style="width:10; height:10;" src="green2.png" alt="Yes"></label>
        </div>

        <div style="width: 100%; margin-top: 13px;">
            <input style="align-content: center; text-align: center; align-content: center;" type="radio" class="2 input-hidden" id="ar112" name="q2" />
            <label for="ar1"><img style="width:10; height:10;" src="red2.png" alt="No"></label>
            <input type="radio" class="2 input-hidden" id="ar2" name="q2" checked />
            <label for="ar2"><img style="width:10; height:10;" src="green2.png" alt="Yes"></label>
        </div>
    </div>
    <div style="width:20%; float:right;">
        <br>
    </div>

    <div style="margin-top: 170px;width: 100%;">
        <p style="text-align: center; font-size: 18px;"><b>On a scale of 1 - 10, .....</b></p>
    </div>

    <div style="width: 5%; float:left;"><br></div>
    <div style="width: 17%; float:left;">
        <textarea style="font-size: 15px; height: 50px;" placeholder=" Text 1"></textarea>
    </div>
    <div style="width: 7%;"></div>
    <div style="width: 7%; float:left; margin-left: 40px;">
        <input type="radio" name="gender" value="male" style="font-size: 18px;"><br>&nbsp; 1</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="male" style="font-size: 18px;"><br>&nbsp; 2</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="male" style="font-size: 18px;"><br>&nbsp; 3</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="male" style="font-size: 18px;"><br>&nbsp; 4</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="male" style="font-size: 18px;"><br>&nbsp; 5</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="male" style="font-size: 18px;"><br>&nbsp; 6</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="male" style="font-size: 18px;"><br>&nbsp; 7</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="male" style="font-size: 18px;"><br>&nbsp; 8</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="male" style="font-size: 18px;"><br>&nbsp; 9</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="female" style="font-size: 18px;"><br>&nbsp; 10</div>

    <div style="margin-top: 95px;width: 100%;">
        <p style="text-align: center; font-size: 18px;"><b>On a scale of 1 - 10, .....</b></p>
    </div>

    <div style="width: 5%; float:left;"><br></div>
    <div style="width: 17%; float:left;">
        <textarea style="font-size: 15px; height: 50px;" placeholder=" Text 2"></textarea>
    </div>
    <div style="width: 7%;"></div>
    <div style="width: 7%; float:left; margin-left: 40px;">
        <input type="radio" name="q3" value="male" style="font-size: 18px;"><br>&nbsp; 1</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q3" value="male" style="font-size: 18px;"><br>&nbsp; 2</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q3" value="male" style="font-size: 18px;"><br>&nbsp; 3</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q3" value="male" style="font-size: 18px;"><br>&nbsp; 4</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q3" value="male" style="font-size: 18px;"><br>&nbsp; 5</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q3" value="male" style="font-size: 18px;"><br>&nbsp; 6</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q3" value="male" style="font-size: 18px;"><br>&nbsp; 7</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q3" value="male" style="font-size: 18px;"><br>&nbsp; 8</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q3" value="male" style="font-size: 18px;"><br>&nbsp; 9</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="female" style="font-size: 18px;"><br>&nbsp; 10</div>


    <div style="margin-top: 95px;width: 100%;">
        <p style="text-align: center; font-size: 18px;"><b>On a scale of 1 - 10, .....</b></p>
    </div>

    <div style="width: 5%; float:left;"><br></div>
    <div style="width: 17%; float:left;">
        <textarea style="font-size: 15px; height: 50px;" placeholder=" Text 3"></textarea>
    </div>
    <div style="width: 7%;"></div>
    <div style="width: 7%; float:left; margin-left: 40px;">
        <input type="radio" name="q4" value="male" style="font-size: 18px;"><br>&nbsp; 1</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q4" value="male" style="font-size: 18px;"><br>&nbsp; 2</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q4" value="male" style="font-size: 18px;"><br>&nbsp; 3</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q4" value="male" style="font-size: 18px;"><br>&nbsp; 4</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q4" value="male" style="font-size: 18px;"><br>&nbsp; 5</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q4" value="male" style="font-size: 18px;"><br>&nbsp; 6</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q4" value="male" style="font-size: 18px;"><br>&nbsp; 7</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q4" value="male" style="font-size: 18px;"><br>&nbsp; 8</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="q4" value="male" style="font-size: 18px;"><br>&nbsp; 9</div>
    <div style="width: 7%; float:left;">
        <input type="radio" name="gender" value="female" style="font-size: 18px;"><br>&nbsp; 10</div>




    <div id="wrapper" style="color: black; margin-top: 93px;">
        <p style="text-align: center; font-size: 18px;">Please provide any details ... & give us feedback ...</p>

        <div style="width: 19%; float:left;">&nbsp;</div>
        <div style="width: 61%; float:left; margin-top: -7px;"><textarea style="width: 100%; height:54px; font-size: 16px;"></textarea></div>
        <div style="width: 20%; float:right;">&nbsp;</div>

        <div>&nbsp;</div>
        <div>&nbsp;</div>


        <div style="width: 100%; display: flex; justify-content: center; margin-top: 20px;">
            <button id="submit" style="border-radius: 10px;; padding-left: 26px; padding-right: 26px; padding-bottom: 5px; padding-top: 5px; background: #4da6ff; color: white; font-size: 23px;">Submit</button>
        </div>

    </div>



</body></html>
