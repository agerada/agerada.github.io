---
title: "Setting up VS Code and R for remote development"
date: 2023-06-15
categories:
  - R
---

RStudio is my almost always my go-to IDE for using R. However, although it is possible to use R through a remote machine through RStudio, many features are lost, such as the workplace viewer. To use remote R through RStudio, start a terminal session, log into the remote environment through SSH, and activate R. Then use `control + option + enter` to dispatch lines of code, instead of `control + enter`. 

VSCode in general is much better suited for integrated remote developmnet, and when [set up](https://code.visualstudio.com/docs/remote/ssh) can be very seamless. I'll be exploring how well this can be extended to R. I'll also need to use R within a conda environment so additional work is needed. 

The [official documentation](https://code.visualstudio.com/docs/languages/r) helps get us started. 

1. Ensure that you have a conda environment with R installed
2. Install `languageserver` using `install.packages("languageserver")` in the loaded conda environment R. Alternatively install `languageserver` using conda-forge: `conda install -c conda-forge r-languageserver`
3. Install the R extension for VS Code __onto the remote server__
4. Install [radian](https://github.com/randy3k/radian), ideally by using conda-forge `conda install -c conda-forge radian`
5. This [forum post](https://github.com/REditorSupport/vscode-R/issues/946) has some useful tips, but when loading radian I was not able to get it to use the conda environment R. This can be fixed by using the following configartion for the R extension on the remote host: 

```
{
    "r.rpath.linux": "path_to_conda/.conda/envs/env_name/bin/R", 
    "r.rterm.linux": "path_to_conda/.conda/envs/env_name/bin/radian",
    "r.rterm.option": [
        "--no-save",
        "--no-restore",
        "--r-binary=path_to_conda/.conda/envs/env_name/bin/R"
    ]
}
```

This forces radian to use the conda R on load. If unsure as to the above paths, make sure that conda environment is activated, and use:

```
which R
which radian
```

6. Now we can finally start an R session using the command pallet (`command + shift + p`) and `Create R terminal` and we should be in the correct version. Workspace viewer, linting, etc, should work. 

I'll update this post if I come across any limitations or a better way to do this. 
