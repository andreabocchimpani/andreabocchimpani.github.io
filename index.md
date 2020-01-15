<h1 align = 'center'> Welcome to Andrea Bocchimpani Github Page </h1>

<div style="text-align:justify">
Mi chiamo Andrea e sono un programmatore di 26 anni. Tutto è iniziato quando fin da piccolo sono rimasto affascinato dal mondo dell'informatica e ho deciso che "da grande" ne avrei fatto parte. Ho studiato informatica e programmazione a scuola e ho potuto imparare le basi di parecchi linguaggi che ho deciso di coltivare in autonomia a casa con piccoli progetti.
Recentemente ho partecipato a due corsi che mi hanno permesso di ampliare e aggiornare le mie competenze nel campo. 
</div>

### Protocol Project

Our task is to build a web application that will have to manage and show a company's protocols. 

We divided the projects in two side:
- Back-End
- Front-End


### Back-End Side

Our first step was to create a class Mail. 
Mail Class have ProtId prop as primary key and a Type prop as Enum in order to have different type of Mail

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

 public enum Tipo
    {
        Entrata = 1,
        Uscita = 2,
        Interna = 3
    }
```

Then we proceeded to create our Database Context:

```
public class ProgettoFinaleContext : DbContext
    {
        public DbSet<Mail> Mails { get; set; }
        protected override void OnConfiguring(DbContextOptionsBuilder optionsBuilder)
        {
            optionsBuilder.UseSqlServer(@"Data Source=(localdb)\MSSQLLocalDB;Initial Catalog=pippo;Trusted_Connection=True;MultipleActiveResultSets=true");
        }
        
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
