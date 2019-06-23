---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Test Post"
subtitle: "Testing the Hugo Academic Theme"
summary: "Post created for Testing the Hugo Academic Theme"
authors: [dbj]
tags: [test]
categories: []
date: 2019-06-23T03:53:13+02:00
lastmod: 2019-06-23T03:53:13+02:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Featured Image"
  focal_point: "smart"
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["my-mermaid-diagrams"]
---

## To create a blog/news article:

       hugo new  --kind post post/my-article-name

Then edit the newly created file content/post/my-article-name.md with your full title and content.

Hugo will automatically generate summaries of posts that appear on the homepage. If you are dissatisfied with an automated summary, you can either limit the summary length by appropriately placing <!--more--> in the article body, or completely override the automated summary by adding a summary parameter to the +++ preamble such that:

     summary: "Summary of my post."

To disable commenting for a specific post, you can add 

    disable_comments: true 

to the post +++ preamble. Or to disable commenting for all posts, you can either set 

      disqusShortname = "" 

in config.toml or 

      disable_comments = true 
      
in params.toml.