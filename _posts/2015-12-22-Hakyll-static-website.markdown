---
layout: post
title: Build a Static Website with Hakyll and Github
date:   2015-12-22 17:11:36 -0800
comments: true
categories: jekyll update
---

Static websites are easy to build, deploy and present your ideas worldwide. In this post we will present the steps used to create a static website using version control.

To do it we used [Hakyll](http://jaspervdj.be/hakyll/index.html) a Haskell library for generating static websites and [Github](http://github.com/) for hosting the static website.

## Steps:

### Hakyll:

  1.  Visit the [Hakyll](http://jaspervdj.be/hakyll/index.html) website.

  2.  Follow the [Installation](http://jaspervdj.be/hakyll/tutorials/01-installation.html) tutorial by *Jasper Van der Jeugt* in the [tutorials](http://jaspervdj.be/hakyll/tutorials.html) tab.

  3.  Follow the instructions of the tutorial, which involves the use of cabal.
      - Optional: Here is a way on how to install a [cabal](https://wiki.haskell.org/Cabal/How_to_install_a_Cabal_package) package.
      - Cabal is a command line tool which is part of the [Haskell platform](https://www.haskell.org/platform/), make sure that the platform is installed first.

  4.  Once you have installed Hakyll Build the example Site which follows the [Installation](http://jaspervdj.be/hakyll/tutorials/01-installation.html) tutorial.

      - if ```hakyll-init my-site``` is not found then make sure <code>&#36;HOME/.cabal/bin</code> is in your <code>$PATH</code>.

      - for OS X <code>&#36;HOME/.cabal</code>. In this case, check <code>&#36;HOME/Library/Haskell/bin</code> and put it on your path if you find hakyll-init there.

      - Here is a way to do this:

      - Be in your home directory:
        <code>cd ~</code>

      - See if <code>.bash_profile</code> exists: <code>ls -al .b*</code>

      - If it does not, create one with your text editor.

      - I used vim, <code>vim ~/.bash_profile</code>

      - Add this line of text to .bash_profile export <code>PATH=$PATH:/Library/Haskell/bin</code>

      - Save and restart the terminal.

  5. After you have built the example website. You can have a look at your website here [http://localhost:8000/](http://localhost:8000/). You can follow the remaining tutorials at Hakyll to customize your website.

### Github:

**Note: [Install git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) first before you attempt to use it.**

  1. Create a new [Github account](https://help.github.com/articles/signing-up-for-a-new-github-account/) if you do not have one.

  2. Create a new [repository](https://help.github.com/articles/create-a-repo/) named <code>username.github.io</code>. Use your github username as the username.

  3. Make an empty directory on your local machine and move into that directory:
      <pre>
      <code>
      mkdir username.github.io
      </code>
      </pre>
      <pre>
      <code>
      cd username.github.io
      </code>
      </pre>

  4. Copy all the contents of your site generated in the previous step of this post.

  5. Finally upload your site on GitHub (this methodology was inspired and partially adopted by Linus Arver Using Hakyll with GitHub [wesite](http://funloop.org/post/2013-01-11-using-hakyll.html)).
      - Move into the <code>_site</code> directory.

      - Initialize a <code>git</code> repository

      - Add all files in that directory.

      - Commit your changes.

      - Specify the remote handle.

      - Push your commits to the origin server.

<pre>
    <code>
cd _site
git init
git add *.html # add css, etc.
git commit -m "initial import"
git remote add origin https://github.com/username/username.github.io.git
git push -u origin master
</code>
</pre>

  6.  Visit <code>username.github.io</code> to view your website.


[Here is a short tutorial on how to link your domain to Github using GoDaddy.](https://medium.com/@LovettLovett/github-pages-godaddy-f0318c2f25a#.ub64k38ot)
