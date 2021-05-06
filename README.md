## Description

Base Binder environment with several visualization packages.

Launch your content repo using [nbgitpuller.link]([nbgitpuller.link](http://nbgitpuller.link?tab=binder&repo=https://github.com/egparedes/base_binder_envs&branch=visualization)



## General instructions

Base Binder environments to be used together with [nbgitpuller](https://github.com/jupyterhub/nbgitpuller) to reduce Binder launch time (as explained in this [blog post](https://discourse.jupyter.org/t/tip-speed-up-binder-launches-by-pulling-github-content-in-a-binder-link-with-nbgitpuller/922)).


### Using this repository as base environment for Binder

To open another GitHub repo as interactive content on Binder using this repository as base environment, use an URL link like: 

`https://mybinder.org/v2/gh/<gh-user-name>/<base-repo-name>/<branch_name>master?urlpath=git-pull?repo=<git-content-repo-url>`

Extra options that can be added to the URL to customize the access to the content repo:

    # Select content-repo branch
    &branch=<git-content-branch>

    # Serve a specific file in content-repo
    &urlpath=<git-content-repo-root>/<full-path-to-file>

    # Open a specific file in classic Jupyter Notebook
    &urlpath=/tree/<git-content-repo-root>/<full-path-to-file>

    # Open a specific file in JupyterLab
    &urlpath=/lab/tree/<git-content-repo-root>/<full-path-to-file>


The recommended (and simpler) way is to the use [nbgitpuller.link](http://nbgitpuller.link?tab=binder&repo=https://github.com/egparedes/base_binder_envs) online tool to generate this composite URL.

The Binder SVG Badge ![Binder](https://mybinder.org/badge.svg) link: https://mybinder.org/badge.svg


### Regular Binder opening

To open a GitHub repo on Binder normally use an URL link like: `https://mybinder.org/v2/gh/<gh-user-name>/<repo-name>.git/<branch_name>`

Example: [https://mybinder.org/v2/gh/egparedes/base_binder_envs.git/master](https://mybinder.org/v2/gh/egparedes/base_binder_envs.git/master)
