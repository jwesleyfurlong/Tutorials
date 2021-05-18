# Tutorials

Primary resources: 
https://bookdown.org/yihui/blogdown/netlify.html
https://alison.rbind.io/post/new-year-new-blogdown/ 
https://happygitwithr.com/rmd-test-drive.html 

1: Create a new repository on github
2: R Studio: Create new project > version control > git
3: R Studio: library(blogdown) > new_site(theme = "wowchemy/starter-academic")
4: Commit new site to github with: usethis::use_git()
5: Netlify: New site from git > continuous deployment > github 
6: rstudioapi::navigateToFile("config.yaml", line = 3)
7: blogdown::config_netlify() & hugo()

