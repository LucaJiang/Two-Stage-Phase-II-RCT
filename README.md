# Instruction on how to use markdown to generate slides

**IMPORTANT:** This repo has set up the github action to automatically generate the slides html file which is pushed to the master branch.

## Write content in [index.md](index.md)

Use this notation to split slides:

```{markdown}
--------------------
```

More than 4 `-` will be treated as a slide separator.

## Convert markdown to slides html

Run the generate.sh under this directory

```sh
sh generate.sh
```

> This generate.sh is only tested on macos.

If success, the presentation will be opened automatically in your browser.

<!-- ### Usage of reveal.js

```sh
git clone https://github.com/hakimel/reveal.js.git
cd reveal.js
git checkout 3.5.0
cd ..
``` -->

## View online

You can view the presentation online at [Two-Stage-Phase-II-RCT](https://lucajiang.github.io/Two-Stage-Phase-II-RCT/)

## Format of Adding Images

```pure
<center><img src="../img/xxx.png" style="zoom:.4"></center>
or
![name](../img/xxx.png)
```

## Reference

1. [nbformat doc](https://nbconvert.readthedocs.io/en/latest/usage.html)

1. [Present your data science projects with Jupyter slides](https://medium.com/learning-machine-learning/present-your-data-science-projects-with-jupyter-slides-75f20735eb0f)

<!-- [3.] [Markdown Cheatsheet]( -->