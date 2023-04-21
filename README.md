# netmastery

## Organization and User Pages
User and Organization Pages sites are not tied to a specific project, and the site files are deployed to the master branch in a dedicated repository named with the GitHub account name. Therefore, you need working copies of two repositories on our local system. For example, consider the following file structure:

```
my-project/
    mkdocs.yml
    docs/
orgname.github.io/
```

After making and verifying updates to your project you need to change directories to the orgname.github.io repository and call the mkdocs gh-deploy command from there:

```
cd ../orgname.github.io/
mkdocs gh-deploy --config-file ../my-project/mkdocs.yml --remote-branch master
```

Note that you need to explicitly point to the mkdocs.yml configuration file as it is no longer in the current working directory. You also need to inform the deploy script to commit to the master branch. You may override the default with the remote_branch configuration setting, but if you forget to change directories before running the deploy script, it will commit to the master branch of your project, which you probably don't want.
