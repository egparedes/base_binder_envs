Base Binder environments to be used together with [nbgitpuller](https://github.com/jupyterhub/nbgitpuller) to reduce Binder launch time (as explained in this [blog post](https://discourse.jupyter.org/t/tip-speed-up-binder-launches-by-pulling-github-content-in-a-binder-link-with-nbgitpuller/922)).


## Using this repository as base environment for Binder

To open another GitHub repo as interactive content on Binder using this repository as base environment use URL link like: 

`https://mybinder.org/v2/gh/<gh-user-name>/<base-repo-name>.git/<branch_name>master?urlpath=git-pull?repo=<git-content-repo-url>

Extra options that can be added to URL to customize aspects of the access to the content repo are:

    # Select content-repo branch
    &branch=<git-content-branch>

    # Serve a specific file in content-repo
    &urlpath=<git-content-repo-root>/<full-path-to-file>

    # Open a specific file in classic Jupyter Notebook
    &urlpath=/tree/<git-content-repo-root>/<full-path-to-file>

    # Open a specific file in JupyterLab
    &urlpath=/lab/tree/<git-content-repo-root>/<full-path-to-file>

[nbgitpuller.link](http://nbgitpuller.link) is an online tool to generate this composite URL easily.

![Binder](https://mybinder.org/badge.svg)] Binder SVG Badge: https://mybinder.org/badge.svg


### Regular Binder opening

To open a GitHub repo on Binder normally use an URL link like: `https://mybinder.org/v2/gh/gh_user_name/repo_name.git/branch_name`

Example: [https://mybinder.org/v2/gh/egparedes/base_binder_envs.git/master](https://mybinder.org/v2/gh/egparedes/base_binder_envs.git/master)

Badge: [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/egparedes/base_binder_envs.git/master)
