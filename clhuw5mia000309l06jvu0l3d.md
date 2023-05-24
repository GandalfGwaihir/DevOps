---
title: "Pushing Your Code to GitHub: A Beginner's Guide to Share Your Code with the World"
datePublished: Fri May 19 2023 18:25:41 GMT+0000 (Coordinated Universal Time)
cuid: clhuw5mia000309l06jvu0l3d
slug: pushing-your-code-to-github
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1684520517928/2c8b3745-9d26-4519-8153-78700a797a54.jpeg
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1684520675268/49d95e84-88ef-43c7-b94a-8961d641941d.jpeg
tags: github, opensource, git

---

  
Imagine waking up one fine day with the determination to share your code with the entire world through open-source. Luckily, there's an incredible platform called GitHub that can turn your aspiration into a reality.

GitHub, being a web-based platform, serves as a hub for version control and collaboration in software development. Its array of powerful features makes it an indispensable tool for developers. With GitHub, you can effortlessly share your codebase with the world, engage in seamless collaboration with fellow developers, and actively contribute to the thriving open-source community.

### Prerequisites:

1. GitHub Account: To make your code open source and share it with the world, you will need to create a GitHub account. Don't worry if you don't have one yet, creating a GitHub account is a straightforward process, **just click here to** [***signup***](https://github.com/signup)*.*
    
2. Git On Local Machine: Git is a free and open-source distributed version control system that enables software developers to manage and track changes made to their source code over time. **If you don't have Git currently installed then you can download and install git from** [***here***](https://git-scm.com/downloads)***.***
    

### Creating A Repository On Github:

To begin creating a new repository for your project, navigate to your GitHub account. On the top right corner, you'll find a `+` button located next to your profile icon. Click on this button to reveal a dropdown menu, and from the options provided, select `New repository`. This action will initialize the process of setting up a fresh repository specifically for your project.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684517422043/638c3607-06e7-4157-8c3f-0182e6b45fa1.png align="center")

Once you click on "New repository," you will be redirected to a new page where you can name your repository. In this example, we have chosen to name it `First Contribution`. It's important to note that GitHub does not allow multiple repositories with the same name within a single account, so make sure to select a unique name for your repository.

For this tutorial, we will set our repository to be public, meaning it will be accessible to anyone. We will keep all the other options at their default values. Once you have finalized the repository settings, scroll down to the bottom of the page and click on the `Create repository` button. This action will create your repository with the specified settings.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684517469982/2c71d14b-a902-4c03-9e6b-fdbc4be1d977.png align="center")

We have initialized an empty repository successfully, now just copy the URL ending with `.git` as seen in the image below.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684517633274/771d0bcf-7547-4683-a9cc-a63523aa1590.png align="center")

We have successfully created our first-ever GitHub repository, yay 🥳  
  
Take a deep breath and appreciate yourself for coming so far!

### Pushing Our Local Code On Github:

Now it's time to push your code to GitHub! Let's begin by opening the folder you want to upload in your preferred IDE, such as Visual Studio Code. Feel free to use any IDE that you're comfortable with for this step.  

To proceed, open the terminal window within your IDE. Once the terminal is open, you can use the command:

```bash
 git init 
```

It initializes a new Git repository. This command creates a new, empty Git repository in the current directory or in the directory you specify. As a result, a `.git` directory will be created in your project directory. This directory holds the repository's metadata and configuration files.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684518149339/6c2f4ab6-4359-443c-99fa-3a7727137587.png align="center")

By default, Git creates a main/master branch, which serves as the primary branch for development within the repository. Branches allow you to work on new features, bug fixes, or experiments without directly affecting the main codebase.

To establish a link between your local repository and the newly created repository on GitHub, you can use the following command:

```bash
git remote add origin <url>
```

This command establishes the link between your local repository and the remote repository. By convention, "origin" is the default name given to the remote repository, but you can opt for a different name if you prefer.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684520645313/c59b6cb5-de95-44a2-8808-17fb7ad610e6.png align="center")

  
To add all the files to the Git staging area, use the command:

```bash
git add .
```

This command allows you to add changes or new files to the staging area. The staging area acts as a space where you can prepare your changes before committing them to the Git repository. By using `git add .`, you include all modified and new files in the staging area, making them ready for the next commit.  
  
After adding files, we can see them by using the command, `git status` :

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684518304962/55a8b2a6-77b7-4817-9f62-8e97c1dbf3c3.png align="center")

  
Now it's time to commit our changes to the main branch of our repository. To do this, we'll use the following git command:

```bash
  git commit -m "Message"
```

When executing this command, make sure to replace "Message" with a descriptive message that summarizes the changes you made with this commit. Adding a meaningful message helps with easy identification and understanding of the changes made in the commit.  

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684518577286/aa8b585e-81a1-45ab-8b44-71609665fa0f.png align="center")

  
Commits play a crucial role in tracking changes within your files. Each commit is assigned a unique ID, which helps in identifying and referencing specific changes. To view the commit history and track changes, you can use the following command:

```basic
git log
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684518717552/69c6333f-c23f-4dee-a6b6-63b8c5b96ece.png align="center")

You guys have come so far and you all really deserve a clap 👏, I would say have a mini fan moment for yourself 😉  
  
Okay now moving onto our last step, we'll push all the changes we have locally committed to the master branch of our GitHub repository, for this purpose we'll use the command:

```bash
git push origin main 
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684519124376/fc60d976-5fa6-4f28-b33b-997cf5f5eb3d.png align="center")

Finallt we can see the local repository on our GitHub:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684519192316/07e57d53-bdc2-4dfb-b675-51bfd0d41df1.png align="center")

  
Congratulations to everyone on successfully making your first contribution on GitHub! This blog served as a stepping stone to enter the exciting world of open source. I highly encourage you to continue exploring different features such as pull requests, issues, and organizations and actively engage with the community.

I hope this blog has provided you with a clear understanding of how to publish your work on GitHub. Thank you for reading all the way through, and I wish you the best of luck on your open-source journey! Remember, the open-source community is waiting to embrace your contributions. Happy coding and best of luck! ❤️