<h1 align="center">Enervoid Theme</h1>

<p align="center">
  A simple black theme for Hugo with KaTeX & mermaid support.   
</p>

<p align="center">
  <img src="https://img.shields.io/github/license/Enerhim/enervoid-theme?color=blue"/>
</p>

[Demo Site](https://enerhim.github.io/enervoid-demo/)

## Images
<details>
<summary>Lists</summary>
  
### Home:
<img width="1920" height="1080" alt="Enervoid Home" src="https://github.com/user-attachments/assets/224c0d55-1705-4824-86fe-6b7c49682031" />

### Blog / Personal:
<img width="1920" height="1080" alt="Enervoid Blog / Personal" src="https://github.com/user-attachments/assets/56a484c5-b3bb-478a-859f-f862bbb3a2b6" />

### Projects:
<img width="1920" height="1080" alt="Enervoid Projects" src="https://github.com/user-attachments/assets/62ba3d14-2764-4a6a-a60f-f64157583cf9" />
</details>
<details>
<summary>Markdown</summary>
  
### Math / Katex
<img width="1920" height="1080" alt="KaTex" src="https://github.com/user-attachments/assets/63f3dfbd-3d41-46b1-b265-d7eef9678eb3" />

### Formattings
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/59765ecc-b26a-4a66-87f9-d1aa9d27381f" />

### Code / Mermaid
<img width="1920" height="1080" alt="Code" src="https://github.com/user-attachments/assets/d181782a-e169-4d5d-96ae-c6ef19712a28" />

### Embeds
<img width="1920" height="1080" alt="Embeds" src="https://github.com/user-attachments/assets/3ee06cff-ce39-4445-b4ab-2aa6fc2488be" />
</details>



## Installation

1. **Create a new Hugo site** (or use existing):
   ```bash
   hugo new site my-site
   cd my-site
   ```

2. **Install the theme** using Git submodule:
   ```bash
   git init
   git submodule add https://github.com/Enerhim/enervoid-theme.git themes/enervoid
   ```

   Or clone it directly:
   ```bash
   git clone https://github.com/Enerhim/enervoid-theme.git themes/enervoid
   ```

4. **Configure your site** — Copy the example configuration:
   ```bash
   cp themes/enervoid/example/hugo.toml ./hugo.toml
   ```

5. **Start Hugo server**:
   ```bash
   hugo server -D
   ```

6. **Visit** `http://localhost:1313` in your browser.



## Configuration

The default `hugo.toml` configuration file:

```toml
baseURL = 'https://example.com'
languageCode = 'en-us'
title = "Your Name"
theme = "enervoid"

[menus]
  [[menus.main]]
    name = 'Blog'
    pageRef = '/blog'
    weight = 10

  [[menus.main]]
    name = 'Personal'
    pageRef = '/personal'
    weight = 20

  [[menus.main]]
    name = 'Projects'
    pageRef = '/projects'
    weight = 30

[params]
  avatar = "https://picsum.photos/200"

  [[params.socials]]
      link = "https://github.com/yourgithub"
      icon = "devicon-github-original"
  [[params.socials]]
      link = "https://twitter.com/yourx"
      icon = "devicon-twitter-original"
   [[params.socials]]
      link = "https://linkedin.in/yourlinkedin"
      icon = "devicon-linkedin-plain"
    [[params.socials]]
      link = "https://itch.io/profile/youritch"
      icon = "fa-brands fa-itch-io" 

[markup]
  [markup.goldmark]
    [markup.goldmark.extensions.passthrough]
      enable = true
      [markup.goldmark.extensions.passthrough.delimiters]
        block = [['$$','$$'], ['\\[','\\]']]
        inline = [['$','$'], ['\\(','\\)']]

    [markup.goldmark.parser]
      [markup.goldmark.parser.attribute]
        block = true

[markup.highlight]
  noClasses = true
  codeFences = true
  guessSyntax = true
  tabWidth = 4
  style = "monokai"
```

For markdown configuration,
- For katex/ math, see [math.md](https://github.com/Enerhim/enervoid-theme/blob/main/content/blog/math.md?plain=1) 
- For formatting, see [formats.md](https://github.com/Enerhim/enervoid-theme/blob/main/content/blog/formats.md?plain=1)
- For images and embeds, see [embeds.md](https://github.com/Enerhim/enervoid-theme/blob/main/content/blog/embeds.md?plain=1)
- For code and mermaid, see [code.md](https://github.com/Enerhim/enervoid-theme/blob/main/content/blog/code.md?plain=1)



## Creating Content

**Blog Post:**
```bash
hugo new blog/my-first-post.md
```

```markdown
+++
title = "My first post"
date = 2024-03-22T14:45:30Z
tags = ["Your", "Tags"]
description = "Your description."
+++

Your content here...
```

Note: Creating a personal post is identical to blog post. Just do 
```bash
hugo new personal/my-personal-post.md
```

**Project:**
```bash
hugo new projects/my-project.md
```

```markdown
+++
title = "My first project"
date = 2024-03-22T14:45:30Z
tags = ["Your", "Project"]
summary = "Your project summary."
github= "Your Github"
website= "Or your website"
link= "Or any other link"
+++

Fallback content
```



## License
This theme is released under the MIT License. See [LICENSE](LICENSE) for details.




