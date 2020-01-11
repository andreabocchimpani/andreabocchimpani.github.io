## Welcome to Andrea Bocchimpani projects site

In this page you cand find some info about our work-group latest project!

### Protocol Project

Our task is to build a web application that will have to manage and show a company's protocols. 

We divided the projects in two side:
- Back-End
- Front-End


### Back-End Side

We start creating a class Mail

```
public class Mail
    {
        [Key]
        public string ProtId { get; set; }
        public string StartDate { get; set; }
        public string ReceiveDate { get; set; }
        public Tipo Type { get; set; }
        public string Sender { get; set; }
        public string Subject { get; set; }
        public string Object { get; set; }
        public string Attachment { get; set; }
    }
```

Our class Mail have ProtId prop as primary key and we create an Enum called Type in order to have different type of Mail

```
public enum Tipo{
        Entrata = 1,
        Uscita = 2,
        Interna = 3
    }
```



```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/andreabocchimpani/andreabocchimpani.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.


### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
