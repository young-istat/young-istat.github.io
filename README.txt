
This document contains notes useful for customization, publication and content management of the website.
Author: Michael Fop


##### favicon.ico to be shown on Chrome tab #####
#
The following files are of interest in order to show the chosen small icon on the Chrome tab. 
	apple-touch-icon.png
	favicon.ico
	favicon-16x16.png
	favicon-32x32.png
These files are in the folder "young_isa_website/themes/cayman-hugo-theme/static/". 
To modify the icon shown on the tab, just change the image of these files, maintaining the names.
#
#####


##### Customizations #####
#
The .scss file "cayman.scss" in the folder "young_isa_website/themes/cayman-hugo-theme/assets/scss" is the principal 
file for customization of the appearance of the website via css coding.
#
#####


##### Fonts from Google Fonts #####
#
Fronts from Google Fonts can be added via the file "head.html" in the folder "young_isa_website/themes/cayman-hugo-theme/layouts/partials".
A selected font can be added simply by copying and pasting from the Google Fonts dedicated html construct link.
#
#####


##### Footer #####
#
Similar to above, the file "footer.html" in the folder "young_isa_website/themes/cayman-hugo-theme/layouts/partials" can be used to change
the layout of the footer at the bottom of each page.
#
#####


##### Landing page #####
#
The content for the landing page is in the file "_index.md" in the folder "young_isa_website/content".
The layout of the landing page is controlled by the file "index.html" in the folder "young_isa_website/themes/cayman-hugo-theme/layouts/partials"
#
#####


##### Push changes to Github from terminal #####
# 
- Navigate to the folder "young_isa_website/public"
- Add changes and modifications and compile them in the "public" folder via the R function "blogdown::serve_site()"
- Add to the "public" folder the file .nojekyll by running from R the code 'file.create("public/.nojekyll")'
- Push to Github:
    git add --all
    git commit -m "somecommit"
    git push -u origin master --force
#
#####


#### Added by Davood on 21.05.2020
To customise the event section and add date, read more etc... the 'list.html' file placed in "website/themes/cayman-hugo-theme/layouts/_default" should be changed. 

also the 'default.md' in "/website/themes/cayman-hugo-theme/archetypes" directroy should be changed as follows:

+++
draft = true
title = ""
summary = ""
date = {{ .Date }}
tags = []
author = ""
+++

###############



