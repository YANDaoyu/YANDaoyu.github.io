# Lagrange

Forked from [LeNPaul/Lagrange](https://github.com/LeNPaul/Lagrange).

Lagrange is a minimalist Jekyll theme for running a personal blog or site for free through [Github Pages](https://pages.github.com/), or on your own server. Everything that you will ever need to know about this Jekyll theme is included in the README below, which you can also find in [the demo site](https://lenpaul.github.io/Lagrange/).

Lagrange 是通过 [Github Pages](https://pages.github.com/) 或者您自己的服务器可建立的最小的个人博客或站点的Jekyll主题。您所需要知道的关于这个Jekyll主题的所有信息都可以在这个README中找到，也可以在 [the demo site](https://lenpaul.github.io/Lagrange/) 中找到。

![alt text](https://user-images.githubusercontent.com/8409329/32631384-17107870-c56e-11e7-932f-deeb7c12e4db.png "Lagrange Demo Image")

## Notable features 主要功能/显著特征

* Compatible with GitHub Pages. 与GitHub Pages兼容。

* Support for Jekyll's built-in Sass/SCSS preprocessor and data files for making customizing easier.
  支持Jekyll内置的Sass/SCSS预处理器和数据文件，使制作更加简单。

* [Google Analytics](https://www.google.com/analytics/) support. 支持 [Google Analytics](https://www.google.com/analytics/) 。

* Commenting support powered by [Disqus](https://disqus.com/). 评论由 [Disqus](https://disqus.com/) 支持。

* Optimized for search engines. 针对搜索引擎进行了优化。

* LaTeX support through [MathJax](https://www.mathjax.org/). 通过 [MathJax](https://www.mathjax.org/) 可支持LaTex。

## Table of Contents 内容表

1. [Introduction 介绍](#introduction)
   1. [What is Jekyll 什么是Jekyll](#what-is-jekyll)
   2. [Never Used Jeykll Before 从未使用过Jekyll](#never-used-jekyll-before)
2. [Installation 安装](#installation)
   1. [GitHub Pages Installation GP安装](#github-pages-installation)
   2. [Local Installation 本地安装](#local-installation)
   3. [Directory Structure 目录结构](#directory-structure)
   4. [Starting From Scratch 从零开始](#starting-from-scratch)
3. [Configuration 配置](#configuration)
   1. [Sample Posts 示例帖](#sample-posts)
   2. [Site Variables 站点变量](#site-variables)
   3. [Adding Menu Pages 添加菜单页](#adding-menu-pages)
   4. [Posts 帖子](#posts)
   5. [Layouts 布局](#layouts)
   6. [YAML Front Block Matter](#yaml-front-block-matter)
4. [Features 特征](#features)
   1. [Design Considerations 设计考虑](#design-considerations)
   2. [Disqus](#disqus)
   3. [Google Analytics](#google-analytics)
   4. [RSS Feeds](#rss-feeds)
   5. [Social Media Icons 社交媒体标识](#social-media-icons)
   6. [MathJax](#mathjax)
   7. [Syntax Highlighting 语法高亮](#syntax-highlighting)
   8. [Markdown](#markdown)
5. [Everything Else 其他](#everything-else)
6. [Contributing](#Contributing)
7. [Questions?](#questions)
8. [Credits](#credits)
9. [License](#license)

## Introduction

Lagrange is a Jekyll theme that was built to be 100% compatible with [GitHub Pages](https://pages.github.com/). If you are unfamiliar with GitHub Pages, you can check out [their documentation](https://help.github.com/categories/github-pages-basics/) for more information. [Jonathan McGlone's guide](http://jmcglone.com/guides/github-pages/) on creating and hosting a personal site on GitHub is also a good resource.

Lagrange 是一个能够完全兼容 [GitHub Pages](https://pages.github.com/) 的Jekyll主题。如果您还不熟悉 GitHub Pages, 您可以参考他们的 [官方文件](https://help.github.com/categories/github-pages-basics/) 来获得更多的资讯。[Jonathan McGlone's guide](http://jmcglone.com/guides/github-pages/) 在创造和管理Github上的个人网站而言也是一个很好的资源。

### What is Jekyll?

Jekyll is a simple, blog-aware, static site generator for personal, project, or organization sites. Basically, Jekyll takes your page content along with template files and produces a complete website. For more information, visit the [official Jekyll site](https://jekyllrb.com/docs/home/) for their documentation. Codecademy also offers a great course on [how to deploy a Jekyll site](https://www.codecademy.com/learn/deploy-a-website) for complete beginners.

Jekyll是一个面向个人、项目、组织站点的简单的、博客感的静态站点生成器。Jekyll可以将您的网页内容和模板文件整合在一起，生成一个完整的网页。若要获得更多的信息，请访问它们的 [官方网站](https://jekyllrb.com/docs/home/)。Codecademy还为纯新手提供了关于 [如何部署Jekyll网站](https://www.codecademy.com/learn/deploy-a-website) 的精彩课程。

### Never Used Jekyll Before? 之前从未用过Jekyll?

The beauty of hosting your website on GitHub is that you don't have to actually have Jekyll installed on your computer. Everything can be done through the GitHub code editor, with minimal knowledge of how to use Jekyll or the command line. All you have to do is add your posts to the `_posts` directory and edit the `_config.yml` file to change the site settings. With some rudimentary knowledge of HTML and CSS, you can even modify the site to your liking. This can all be done through the GitHub code editor, which acts like a content management system (CMS).

在Github上管理您的主页最美妙的地方在于 —— 您实际上不需要在电脑上安装Jekyll。所有事都可以直接通过Github的代码编辑器完成，您只需要有和一点点关于Jekyll和命令行的了解。您需要做的只有添加您的文章到 `_posts` 目录然后编辑 `_config.yml` 文件更改站点的设置。 若您有一些基本的HTML和CSS知识，您还可以根据您的喜好自由更改站点。这都可以通过Github代码编辑器完成，它就像一个内容管理系统(CMS)。

## Installation

### GitHub Pages Installation

To start using Jekyll right away with GitHub Pages, [fork the Lagrange repository on GitHub](https://github.com/LeNPaul/Lagrange/fork). From there, you can rename your repository to 'USERNAME.github.io', where 'USERNAME' is your GitHub username, and edit the `settings.yml` file in the `_data` folder to your liking. Ensure that you have a branch named `gh-pages`. Your website should be ready immediately at 'http://USERNAME.github.io'. Note: if you are hosting several sites under the same GitHub username, then you will have to use [Project Pages instead of User Pages](https://help.github.com/articles/user-organization-and-project-pages/) - just change the repository name to something other than 'http://USERNAME.github.io'.

可以从 [fork the Lagrange repository on GitHub](https://github.com/LeNPaul/Lagrange/fork) 开始来使用Jekyll和GP。在这里，您可以重命名您的仓库名为 'USERNAME.github.io', 其中 'USERNAME' 是您的Github用户名，并且根据喜好编辑 `_data` 文件夹中的 `settings.yml` 。保证您有一个分支名字为 `gh-pages`。您的网站就会马上在 'http://USERNAME.github.io' 处生成。注意：如果您在同一个Github用户名下持有多个站点，那么您需要使用 [Project Pages 代替 User Pages](https://help.github.com/articles/user-organization-and-project-pages/) —— 把您的仓库名改成除了 'http://USERNAME.github.io' 以外的名字。

Head over to the `_posts` directory to view all the posts that are currently on the website, and to see examples of what post files generally look like. You can simply just duplicate the template post and start adding your own content.

转到 `_posts` 目录可以查看当前网站上的所有帖子，并看到这些实例帖子文件大概长什么样。您可以简单地复制模板文章并开始添加自己的内容。

### Local Installation

For a full local installation of Lagrange, [download your own copy of Lagrange](https://github.com/LeNPaul/Lagrange/archive/gh-pages.zip) and unzip it into it's own directory. From there, open up your favorite command line tool, enter `bundle install`, and then enter `jekyll serve`. Your site should be up and running locally at [http://localhost:4000](http://localhost:4000).

完全的本地安装，[下载Lagrange](https://github.com/LeNPaul/Lagrange/archive/gh-pages.zip) 并解压在您自己的文件夹。然后在这里打开您最爱的命令行工具，输入 `bundle install`, 再输入 `jekyll serve`。您的网站就会在 [http://localhost:4000](http://localhost:4000) 启动并运行。

### Directory Structure

If you are familiar with Jekyll, then the Lagrange directory structure shouldn't be too difficult to navigate. The following some highlights of the differences you might notice between the default directory structure. More information on what these folders and files do can be found in the [Jekyll documentation site](https://jekyllrb.com/docs/structure/).

如果您熟悉Jekyll, 那么Lagrange的目录结构就不会太难定位。以下是您可能会注意到的与默认目录结构之间存在差异的一些点。有关这些文件夹和文件的功能的更多信息可以在 [Jekyll文档站点](https://jekyllrb.com/docs/structure/) 中找到。

```bash
Lagrange/
├── _data                      # Data files 数据文件
|  └── settings.yml            # Theme settings and custom text 主题设置和自定义文本
├── _includes                  # Theme includes 主题的includes
├── _layouts                   # Theme layouts (see below for details) 主题布局(详见下文)
├── _posts                     # Where all your posts will go 帖子所在地
├── assets                     # Style sheets and images are found here 样式表和图所在文件夹
|  ├── css                     # Style sheets go here 样式表
|  |  └── main.css             # Main CSS file 主CSS文件
|  |  └── syntax.css           # Style sheet for code syntax highlighting 代码语法高亮的样式表
|  └── img                     # Images go here 图
├── menu                       # Menu pages 菜单页
├── _config.yml                # Site build settings 网站建立设置
├── Gemfile                    # Ruby Gemfile for managing Jekyll plugins 管理Jekyll附件的Ruby Gemfile
├── index.md                   # Home page 主页
├── LICENSE.md                 # License for this theme 主题证书
├── README.md                  # Includes all of the documentation for this theme 关于主题的所有细节
└── rss-feed.xml               # Generates RSS 2.0 file which Jekyll points to 生成Jekyll指向的RSS 2.0文件
```

### Starting From Scratch 从零开始

To completely start from scratch, simply delete all the files in the `_posts`, `assets/img`, and `menu` folder, and add your own content. You may also replace the `README.md` file with your own README. Everything in the `_data` folder and `_config.yml` file can be edited to suit your needs. You may also change the `favicon.ico` file to your own favicon.

如果要完全从零开始，可以直接删掉所有文件夹 `_posts`, `assets/img`, 和 `menu` 内的文件，添加成您自己的文件。您也可以用自己的README替换原有的 `README.md` 。在 `_data` 文件夹里面的文件和 `_config.yml` 文件都可以根据需求更改。您也可以根据需求更改 `favicon.ico` 文件。

## Configuration

### Sample Posts

Visit the [the demo site](https://lenpaul.github.io/Lagrange/) to find sample posts that show what different types of text formatting look like. You can find these posts in the `_posts` folder, which show what the best practices for setting up your own site are.

访问 [the demo site](https://lenpaul.github.io/Lagrange/) 可以得到不同形式的示例帖。这些帖子都可以在 `_posts` 文件夹找到，显示了建立您自己的网站的最佳做法。

### Site Variables

To change site build settings, edit the `_config.yml` file found in the root of your repository, which you can tweak however you like. More information on configuration settings and plugins can be found on [the Jekyll documentation site](https://jekyllrb.com/docs/configuration/). This is also where you will be able to customize the title, description, and the author/owner of your site.

要更改网站构建设置，请编辑存储库根目录中的 `_config.yml` 文件。 有关配置设置和插件的更多信息，请参见 [Jekyll文档站点](https://jekyllrb.com/docs/configuration/)。 这也是您可以自定义网站的标题、说明、作者/所有者的地方。

If you are hosting your site on GitHub Pages, then committing a change to the `_config.yml` file will force a rebuild of your site with Jekyll. Any changes made should be viewable soon after. If you are hosting your site locally, then you must run `jekyll serve` again for the changes to take place.

如果您在GitHub页面上管理您的网站，那么对 `_config.yml` 文件进行更改会强制重建您的网站与Jekyll。 之后所做的任何更改都应该可以查看。 如果您在本地管理您的网站，那么您必须再次运行“jekyll serve”以进行更改。

In the `settings.yml` file found in the `_data` folder, you will be able to customize your site settings, such as setting Disqus comments, Google Analytics, what shows up in your menu, and social media information.

在 `_data` 文件夹中的 `settings.yml` 文件中，您可以自定义您的网站设置，例如设置Disqus评论、Google Analytics、菜单中显示的内容以及社交媒体信息。

### Adding Menu Pages

The menu pages are found in the `menu` folder in the root directory, and can be added to your menu in the `settings.yml` file.

菜单页面位于根目录下的 `menu` 文件夹中，可以在 `settings.yml` 文件中添加到菜单中。

### Posts

You will find example posts in your `_posts` directory. Go ahead and edit any post and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

你会在 `_posts` 目录中找到示例帖。 继续编辑任何帖子并重新构建网站以查看您的更改。 您可以用许多不同的方式重建网站，但最常见的方式是运行 `jekyll serve`, 它启动一个Web服务器并在更新文件时自动重新生成您的网站。

To add new posts, simply add a file in the `_posts` directory that follows the convention of `YYYY-MM-DD-name-of-post.md` and includes the necessary front matter. Take a look at any sample post to get an idea about how it works. If you already have a website built with Jekyll, simply copy over your posts to migrate to Lagrange.

要添加新帖子，只需在符合 `YYYY-MM-DD-name-of-post.md` 约定的 `_posts` 目录中添加一个文件，并包含必要的前置事项。 看示例文章，了解它是如何工作的。 如果您已经有了使用Jekyll建立的网站，只需复制您的帖子即可迁移到Lagrange。

### Layouts

There are two main layout options that are included with Lagrange: post and page. Layouts are specified through the [YAML front block matter](https://jekyllrb.com/docs/frontmatter/). Any file that contains a YAML front block matter will be processed by Jekyll. For example:

Lagrange包含两种主要布局选项：文章和页面。 布局通过 [YAML front block matter](https://jekyllrb.com/docs/frontmatter/) 指定。 任何包含YAML前端问题的文件都将由Jekyll处理。 例如：

```
---
layout: post 布局：文章
title: "Example Post" 标题："示例帖"
---
```

Examples of what posts looks like can be found in the `_posts` directory, which includes this post you are reading right now. Posts are the basic blog post layout, which includes a header image, post content, author name, date published, social media sharing links, and related posts.

您可以在 `_posts` 目录中找到帖子大概长什么样，目录中也包括您正在阅读的这篇文章。帖子是基本的博客布局，其中包括标题图片、帖子内容、作者姓名、发布日期、社交媒体分享链接以及相关帖子。

Pages are essentially the post layout without any of the extra features of the posts layout. An example of what pages look like can be found at the [About](https://lenpaul.github.io/Lagrange/menu/about.html) and [Contacts](https://lenpaul.github.io/Lagrange/menu/contact.html).

页面是最基础的帖子布局，没有任何帖子布局的额外功能。你可以在 [About](https://lenpaul.github.io/Lagrange/menu/about.html) 和 [Contacts](https://lenpaul.github.io/Lagrange/menu/contact.html) 中看到页面长什么样。

In addition to the two main layout options above, there are also custom layouts that have been created for the [home page](https://lenpaul.github.io/Lagrange/) and the [archives page](https://lenpaul.github.io/Lagrange/menu/writing.html). These are simply just page layouts with some [Liquid template code](https://shopify.github.io/liquid/). Check out the `index.html` file in the root directory for what the code looks like.

除上述两个主要布局选项之外，还有为 [主页](https://lenpaul.github.io/Lagrange/) 和 [档案页面](https://lenpaul.github.io/Lagrange/menu/writing.html) 创建的自定义布局。这些仅仅是带有一些 [Liquid模板代码](https://shopify.github.io/liquid/) 的页面布局。 查看根目录下的 `index.html` 文件可了解代码的样子。

### YAML Front Block Matter

The recommended YAML front block is:
推荐的YAML前端是：

```
---
layout:
title:
author:
categories:
tags: []
image:
---
```

`layout` specifies which layout to use, `title` is the page or post title, `categories` can be used to better organize your posts, `tags` are used when generating related posts based on the topic of the post, and `image` specifies which images to use. Have a look at some posts in the `_posts` directory to see how these variables are set.

`layout` 指定要使用哪种布局，`title` 是页面或帖子标题，可以使用 `categories` 更好地组织帖子，当根据帖子主题生成相关帖子时使用 `tags`, `image` 指定要使用的图像。 看看 `_posts` 目录中的一些帖子，看看这些变量是如何设置的。

## Features

### Design Considerations

Lagrange was designed to be a minimalist theme in order for the focus to remain on your content. For example, links are signified mainly through an underline text-decoration, in order to maximize the perceived affordance of clickability (I originally just wanted to make the links a darker shade of grey).

### Disqus

Lagrange supports comments at the end of posts through [Disqus](https://disqus.com/). In order to activate Disqus commenting, set `disqus.comments` to true in the `_data/settings.yml` file. If you do not have a Disqus account already, you will have to set one up, and create a profile for your website. You will be given a `disqus_shortname` that will be used to generate the appropriate comments sections for your site. More information on [how to set up Disqus](http://www.perfectlyrandom.org/2014/06/29/adding-disqus-to-your-jekyll-powered-github-pages/).

### Google Analytics

It is possible to track your site statistics through [Google Analytics](https://www.google.com/analytics/). Similar to Disqus, you will have to create an account for Google Analytics, and enter the correct Google ID for your site under `google-ID` in the `settings.yml` file. More information on [how to set up Google Analytics](https://michaelsoolee.com/google-analytics-jekyll/).

### RSS Feeds

Atom is supported by default through [jekyll-feed](https://github.com/jekyll/jekyll-feed). With jekyll-feed, you can set configuration variables such as 'title', 'description', and 'author', in the `_config.yml` file.

RSS 2.0 is also supported through [RSS auto-discovery](http://www.rssboard.org/rss-autodiscovery). The `rss-feed.xml` file (based on the template found at [jekyll-rss-feeds](https://github.com/snaptortoise/jekyll-rss-feeds)) that the feed path points to when using RSS 2.0 is automatically generated based on the appropriate configuration variables found in `_data/settings.yml`.

To use RSS 2.0, ensure the following is done:

* Uncomment the last two lines in the `_config.yml` file.

* In `_data/settings.yml`, under 'social', comment out the rss-square that points to `feed.xml`, and uncomment the rss-square that points to `rss-feed.xml`.

* In `_includes/head.html`, comment out `{% feed_meta %}` and uncomment the line under the RSS 2.0 comment.

### Social Media Icons

All social media icons are courtesy of [Font Awesome](http://fontawesome.io/). You can change which icons appear, as well as the account that they link to, in the `settings.yml` file in the `_data` folder.

### MathJax

Lagrange comes out of the box with [MathJax](https://www.mathjax.org/), which allows you to display mathematical equations in your posts through the use of [LaTeX](http://www.andy-roberts.net/writing/latex/mathematics_1).

### Syntax Highlighting

Lagrange provides syntax highlighting through [fenced code blocks](https://help.github.com/articles/creating-and-highlighting-code-blocks/). Syntax highlighting allows you to display source code in different colors and fonts depending on what programming language is being displayed. You can find the full list of supported programming languages [here](https://github.com/jneen/rouge/wiki/List-of-supported-languages-and-lexers). Another option is to embed your code through [Gist](https://en.support.wordpress.com/gist/).

### Markdown

As always, Jekyll offers support for GitHub Flavored Markdown, which allows you to format your posts using the [Markdown syntax](https://guides.github.com/features/mastering-markdown/). Examples of these text formatting features can be seen below. You can find this post in the `_posts` directory as well as the `README.md` file.

## Everything Else

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll's GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/

## Contributing

If you would like to make a feature request, or report a bug or typo in the documentation, then please [submit a GitHub issue](https://github.com/LeNPaul/Lagrange/issues/new). If you would like to make a contribution, then feel free to [submit a pull request](https://help.github.com/articles/about-pull-requests/) - as a bonus, I will credit all contributors below! If this is your first pull request, it may be helpful to read up on the [GitHub Flow](https://guides.github.com/introduction/flow/) first.

Lagrange has been designed as a base for users to customize and fit to their own unique needs. Please keep this in mind when requesting features and/or submitting pull requests. Some examples of changes that I would love to see are things that would make the site easier to use, or better ways of doing things. Please avoid changes that do not benefit the majority of users.

## Questions?

This theme is completely free and open source software. You may use it however you want, as it is distributed under the [MIT License](http://choosealicense.com/licenses/mit/). If you are having any problems, any questions or suggestions, feel free to [tweet at me](https://twitter.com/intent/tweet?text=My%question%about%Lagrange%is:%&amp;via=paululele), or [file a GitHub issue](https://github.com/lenpaul/lagrange/issues/new).

## Credits

### Creator

#### Paul Le

* [www.lenpaul.com](http://lenpaul.com)

* [Twitter](https://twitter.com/paululele)

* [GitHub](https://github.com/LeNPaul)

### Contributors

* [nikolalukovic](https://github.com/nikolalukovic)

* [gmemstr](https://github.com/gmemstr)

* [lynn9388](https://github.com/lynn9388)

* [robqiao](https://github.com/robqiao)

* [Mauladen](https://github.com/Mauladen)

* [dhanus](https://github.com/dhanus)

* [mlewand](https://github.com/mlewand)

* [Hguimaraes](https://github.com/Hguimaraes)

* [ilhamadun](https://github.com/ilhamadun)

* [brianclemens](https://github.com/brianclemens)

* [leyhline](https://github.com/leyhline)

### Icons + Demo Images

* [Death to Stock](https://deathtothestockphoto.com/)

* [Font Awesome](http://fontawesome.io/)

### Other

* [Jekyll](https://jekyllrb.com/)

* [Free Code Camp](https://www.freecodecamp.org)

* [Khan Academy](https://www.khanacademy.org/)

## License

Open sourced under the [MIT license](https://github.com/LeNPaul/Lagrange/blob/gh-pages/LICENSE.md).
