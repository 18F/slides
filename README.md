# 18F/slides

```
   #    #####               #                                      
  ##   #     # ######      #   ####  #      # #####  ######  ####  
 # #   #     # #          #   #      #      # #    # #      #      
   #    #####  #####     #     ####  #      # #    # #####   ####  
   #   #     # #        #          # #      # #    # #           # 
   #   #     # #       #      #    # #      # #    # #      #    # 
 #####  #####  #      #        ####  ###### # #####  ######  ####  
                                                                   
```
# Why 18F/slides

You should use 18F/slides if you:

1. Can do Markdown,
2. Want a stupidly simple way to hack up a presentation,
3. Want a URL for your slide deck, and
4. Want `git`.

# How to Use 18F/slides

To use 18F/slides:

1. Create a new `.html` file in the `_slides` directory.
2. Add yaml frontmatter to the file with the following:

	```
	---
	layout: default
	path: path-to-url
	title: Title for 18F/slides
	---
	```

3. Create slides, using markdown syntax (technically, it's redcarpet, go nuts).
4. Separate slides using `---` for horizontal pagination between slides and `--` for vertical pagination.
5. Commit the file to the `18f-pages` branch of the 18F/slides repo.
6. Profit. See [the sample slides](https://pages.18f.gov/slides/sample/) to get a feel for how the navigation works.

# How does it work?

18F/slides leverages the amazing open-source [reveal.js](https://github.com/hakimel/reveal.js/) library and [jekyll](https://jekyllrb.com) and is hosted on [18F pages](https://pages.18f.gov/).

# How can I use this for my own slides?
If you'd like to use Slides for your own organization, here are some tips on how to fork it and get your own version:

1. Fork! (of course)
2. Edit _config.yml. Modify title/email and - critically - the "url" field to reflect your GitHub repository, e.g. https://github.com/18F/slides/ becomes https://pages.18f.gov/slides/. Make sure you commit to the 18f-pages branch so 18F Pages picks it up.
3. Wait for a little while - 18F Pages is working behind the scenes for your initial setup,  and if you try to actually view your slides right away, you'll probably get a 404. It sometimes takes 5-10 minutes; once it's set up initially, changes take effect pretty quickly.
4. You'll presumably want to define your own theme, or pick one of the existing ones (take a look in ../assets/css/theme), and edit _layouts/default.html to reflect it. Look for the link with id="theme" in it.
5. That's it! Enjoy your slides.

# How can I make it better?

See [CONTRIBUTING.md](https://github.com/18F/slides/blob/18f-pages/CONTRIBUTING.md).
