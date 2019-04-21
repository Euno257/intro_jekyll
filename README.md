# Introduction to basic jekyll
Making a Static Website using jekyll.

## Install jekyll
<p><code> gem install bundler jekyll </code></p>

## Initialising jekyll
<p><code> jekyll new projectname </code></p>

## Hosting
for first time starting the server
<p><code> bundle exec jekyll serve </code><p>
Otherwise just use
<p><code> jekyll serve </code></p>

## Blogs
More blog can be added by adding .md fies to the 'posts' folder.

## Adding Drafts
Add another folder namely 'drafts'.To this folder you can add important documents which you don't want display on the website.

## Section
Adding other sections like 'Abouts' ection. Add these kind of sections by directly adding markdown files to the main folder.

## Permalink
By using permalink attribute you can assign a URL to any page as of your own choice.

## Themes
Jekyll uses 'minima' as a default theme. You can find different themes on https://rubygems.org/
Take the name of the theme which you want to install and add it to the 'Gemfile' inside the main folder.
  <p><code> gem "ThemeName" </code></p>
 Then stop the server(ctrl+c) and write the command:
 <p><code> bundle install </code></p>
The above command will install all the gem for you. Now lastly you have to add your themename to the 'config.yml' file and its done. That's it!!
Now for results, Start your site server using
<p><code> bundle exec jekyll server </code></p>

#### Just wait a second, I refreshed my page & "we are not getting anything on our server why?"
It's happening because in our new theme, it doesn't contains layouts like 'page','home' & 'post'. So go to your theme's github repository and checkout the layouts folder. Change the layouts in the our websites folder. It's amazing!

## Custom layouts
You can also add a "layout" folder if you want to customize your websites layout.
Add html file inside the folder and specify the file's name in each markdown file's layout section.

## Adding includes
Make a new folder for includes and store the html files in it. let say we want to include header of our website from 'header.html' on a another html file you have to write <p><code> {{% include header.html %}} </code></p>

## Add a mini database to your website
Make a ' data' folder inside the main folder. This folder contains 3 types of data files .yml,.json & .csv format files to store the data.

## for checking on localhost
Change the directory that contains the Gem file.
  Run in terminal <p><code> jekyll serve </code></p>

#### Now our website is ready and if you want to deploy it on github pages, upload all your files to 'gh-pages' branch. Lastly if you liked the tutorial, don't forget to Star!
