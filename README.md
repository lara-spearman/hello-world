## The trial page 

You can use the [editor on GitHub](https://github.com/lara-spearman/hello-world/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
Members should appear here
 
{{ page.title }}
 
{% if page.title %}
 Show {{ page.title }}
{% endif %}
    


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


