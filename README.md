# HighResMIP2 GitHub Pages website

This website is hosted through [GitHub Pages with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll). Basically, this allows pages to be written in [Markdown](https://www.markdownguide.org/tools/jekyll/), which is then converted to static HTML webpages by applying the template included in the repository. The static web pages are then served from https://highresmip.org/.

The pages are hosted in the [gh-pages](https://github.com/HighResMIP2/HighResMIP2.github.io/tree/gh-pages) branch of this repository. You can monitor the building of this branch from markdown into static HTML on the [Actions](https://github.com/HighResMIP2/HighResMIP2.github.io/actions) page. When you are developing the pages locally then you can use Ruby and Jekyll to build and serve these pages locally. 

## Creating a local development environment

It is relatively easy to install Ruby and Jekyll into a Conda environment:

1. Create a Conda environment called Ruby:

    `conda create -n ruby -c conda-forge ruby c-compiler compilers cxx-compiler`

1. Start the environment

    `conda activate ruby`

1. Install Jekyll, bundler and their dependencies into this environment:
    
    `gem install jekyll bundler`

1. Jekyll expects Ruby to be installed into the same Gem, but this doesn't happen in this Conda environment and so manually add an appropriate symlink:
    
    `ln -s <path_to_conda>/envs/ruby/bin/ruby <path_to_conda>/envs/ruby/share/rubygems/bin/ruby` 

1. In Ruby V3 some dependencies aren't installed automatically and so add these:

    `bundle add webrick`
    
1. The above steps only need to be done on the initial creation of the Conda environment. Subsequently the Conda environment can be started with just:

    `conda activate ruby`  
   
1. Change directory to your local copy of the repository:

    `cd <path-to-local-copy-of-repo>`

1. The site can then be rendered and served locally:

    `bundle exec jekyll serve `

    with the site being available from http://127.0.0.1:4000/


## Editing and publishing changes

Users should branch the `gh-pages` branch, develop their changes on their branch, view them locally and then create a pull request to have them merged into the repository and published.

1. Get a local copy of the repository:

    `git clone git@github.com:HighResMIP2/HighResMIP2.github.io.git`

1. Change into the local copy:

    `cd HighResMIP2.github.io`

1. Create a branch:

    `git br <branch-name> origin/gh-pages`

1. Switch to the branch:

    `git co <branch-name>`

1. Make your changes

1. Start the Conda environment (possibly in a new terminal):

    `conda activate ruby`

1. Start Jekyll:

    `bundle exec jekyll serve `

    with the site being available from http://127.0.0.1:4000/ and pages being re-rendered when changes are saved locally, but F5 will have to be pressed in the browser to reload the changes there. Occasionally, when changes are made to a template then the page may not be re-rendered. In this case Jekyll can be stopped by pressing Ctrl-C and starting it again.

1. When all of the changes have been made locally then check which files have been edited:

    `git status`

1. Optionally, use diff to view the changes

    `git diff`

    or
    
    `git difftool`

1. Commit these changes:

    `git commit -am '<Description of changes>'`

1. The commit can be pushed to your branch at GitHub:

    `git push origin <branch-name>`

1. Create a pull request at GitHub by going to https://github.com/HighResMIP2/HighResMIP2.github.io/compare and comparing `<branch-name>` with `gh-pages`.

1. Review (yourself or someone else) the pull request and merge into `gh-pages`.

1. Monitor [GitHub Actions](https://github.com/HighResMIP2/HighResMIP2.github.io/actions) to check that the changes are built, reported and deployed.

1. Your changes should now be available at https://highresmip.org/.


