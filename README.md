# Jekyll Now

## Screenshots
Blog Page (Posts)
![Blog Page](https://github.com/thomasvaeth/trophy/blob/master/_screenshots/screenshot-1.png "Desktop screenshot")

Blog Page (Categories)
![Blog Page](https://github.com/thomasvaeth/trophy/blob/master/_screenshots/screenshot-2.png "Desktop screenshot")

- You don't need to touch the command line
- You don't need to install/configure ruby, rvm/rbenv, ruby gems :relaxed:
- You don't need to install runtime dependencies like markdown processors, Pygments, etc
- If you're on Windows, this will make setting up Jekyll a lot easier
- It's easy to try out, you can just delete your forked repository if you don't like it

Post Page (Profile & Footer)
![Post Page](https://github.com/thomasvaeth/trophy/blob/master/_screenshots/screenshot-4.png "Desktop screenshot")

Archive Page
![Archive Page](https://github.com/thomasvaeth/trophy/blob/master/_screenshots/screenshot-5.png "Desktop screenshot")

## Installation
All dependencies are saved in the ````Gemfile````. Run ````bundle install```` (Install [Bundler](http://bundler.io/) if it is not already) after cloning the repo.

## Edit Theme
I made everything as easy as possible to edit. Most things can be found in the ````_config.yml````, but if more editing is required digging through the code will be required. The ````head.html```` file is in the ````_includes```` folder and the Sass variables are found in the ````_base.scss```` file in the ````_sass```` folder.

### _config.yml

Your Jekyll blog will often be viewable immediately at <https://yourgithubusername.github.io> (if it's not, you can often force it to build by completing step 2)

* ````email```` - Your email for the contact card and the footer
* ````baseurl```` - Path of blog if adding this on to another website
* ````paginate```` - Number of blog posts per page
* ````paginate_path```` - URL structure of paginated pages
* ````google_analytics```` - Option field to replace with correct Google Analytics code

#### SEO Settings
    title: 
    description: 
    url: ""
    twitter_username: 
    default_img: 

* ````title```` - Title of blog
* ````description```` - Description of blog (recommended to not go over 160 characters)
* ````url```` - URL of main website
* ````twitter_username```` - Twitter username
* ````default_img```` - Image that will appear when posting links on social networks

Making a change to _config.yml (or any file in your repository) will force GitHub Pages to rebuild your site with jekyll. Your rebuilt site will be viewable a few seconds later at <https://yourgithubusername.github.io> - if not, give it ten minutes as GitHub suggests and it'll appear soon

* ````name```` - Full name for SEO purposes
* ````profile_img```` - Image for the profile card (size to 2000x1200px)
* ````profile```` - Short description that will be in the profile card
* ````social```` - List of social networks for icons in the contact card and the footer ([Font Awesome](http://fontawesome.io/) is used, so only match the name of the icon, but do not include ````fa-````)


![_config.yml](/images/config.png "_config.yml")

### Step 3) Publish your first blog post

* ````include```` - Folders that are not automatically included in Jekyll
* ````exclude```` - Folders that are excluded from `_site_`
* ````permalink```` - URL structure of blog posts

### _posts
    ---
    layout: post
    title: ""
    date: 
    categories:
    description: 
    image: 
    image-sm:
    ---

This is the YAML front matter block for blog posts.
* ````layout```` - This field will always be post
* ````title```` - The title of the blog post
* ````date```` - The date that will appear on the blog post
* ````categories```` - Optional field that can be entered as an array or a list
* ````description```` - Optional field for SEO (recommended to not go over 160 characters)
* ````image```` - The blog theme was designed for 2000x1200px images (optimize your images because this is a picture heavy theme)
* ````image-sm```` - Optional field for card layouts for image optimization and page speed (designed for 500x300px images)

### _categories
    ---
    layout: default
    title: New Category
    description:
    permalink: /category/new-category/
    ---
    {% include category.html %}

1. Install Jekyll and plug-ins in one fell swoop. `gem install github-pages` This mirrors the plug-ins used by GitHub Pages on your local machine including Jekyll, Sass, etc.
2. Clone down your fork `git clone https://github.com/yourusername/yourusername.github.io.git`
3. Serve the site and watch for markup/sass changes `jekyll serve`
4. View your website at http://127.0.0.1:4000/
5. Commit any changes and push everything to the master branch of your GitHub user repository. GitHub Pages will then rebuild and serve your website.

## Upcoming Additions
* Page transitions
* More styled elements for blog posts

## Issues
Please submit any issues [here](https://github.com/thomasvaeth/trophy/issues).

It covers:

- A more detailed walkthrough of setting up your Jekyll blog
- Common issues that you might encounter while using Jekyll
- Importing from Wordpress, using your own domain name, and blogging in your favorite editor
- Theming in Jekyll, with Liquid templating examples
- A quick look at Jekyll 2.0’s new features, including Sass/Coffeescript support and Collections

## Jekyll Now Features

✓ Command-line free _fork-first workflow_, using GitHub.com to create, customize and post to your blog  
✓ Fully responsive and mobile optimized base theme (**[Theme Demo](http://jekyllnow.com)**)  
✓ Sass/Coffeescript support using Jekyll 2.0  
✓ Free hosting on your GitHub Pages user site  
✓ Markdown blogging  
✓ Syntax highlighting  
✓ Disqus commenting  
✓ Google Analytics integration  
✓ SVG social icons for your footer  
✓ 3 http requests, including your avatar  

✘ No installing dependencies
✘ No need to set up local development  
✘ No configuring plugins  
✘ No need to spend time on theming  
✘ More time to code other things ... wait ✓!  

## Questions?

[Open an Issue](https://github.com/barryclark/jekyll-now/issues/new) and let's chat!

## Other forkable themes

You can use the [Quick Start](https://github.com/barryclark/jekyll-now#quick-start) workflow with other themes that are set up to be forked too! Here are some of my favorites:

- [Hyde](https://github.com/poole/hyde) by MDO
- [Lanyon](https://github.com/poole/lanyon) by MDO
- [mojombo.github.io](https://github.com/mojombo/mojombo.github.io) by Tom Preston-Werner
- [Left](https://github.com/holman/left) by Zach Holman
- [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) by Michael Rose
- [Skinny Bones](https://github.com/mmistakes/skinny-bones-jekyll) by Michael Rose

## Credits

- [Jekyll](https://github.com/jekyll/jekyll) - Thanks to its creators, contributors and maintainers.
- [SVG icons](https://github.com/neilorangepeel/Free-Social-Icons) - Thanks, Neil Orange Peel. They're beautiful.
- [Solarized Light Pygments](https://gist.github.com/edwardhotchkiss/2005058) - Thanks, Edward.
- [Joel Glovier](http://joelglovier.com/writing/) - Great Jekyll articles. I used Joel's feed.xml in this repository.
- [David Furnes](https://github.com/dfurnes), [Jon Uy](https://github.com/jonuy), [Luke Patton](https://github.com/lkpttn) - Thanks for the design/code reviews.
- [Bart Kiers](https://github.com/bkiers), [Florian Simon](https://github.com/vermluh), [Henry Stanley](https://github.com/henryaj), [Hun Jae Lee](https://github.com/hunjaelee), [Javier Cejudo](https://github.com/javiercejudo), [Peter Etelej](https://github.com/etelej), [Ben Abbott](https://github.com/jaminscript), [Ray Nicholus](https://github.com/rnicholus), [Erin Grand](https://github.com/eringrand), [Léo Colombaro](https://github.com/LeoColomb), [Dean Attali](https://github.com/daattali), [Clayton Errington](https://github.com/cjerrington), [Colton Fitzgerald](https://github.com/coltonfitzgerald), [Trace Mayer](https://github.com/sunnankar) - Thanks for your [fantastic contributions](https://github.com/barryclark/jekyll-now/commits/master) to the project!

## Contributing

Issues and Pull Requests are greatly appreciated. If you've never contributed to an open source project before I'm more than happy to walk you through how to create a pull request.

You can start by [opening an issue](https://github.com/barryclark/jekyll-now/issues/new) describing the problem that you're looking to resolve and we'll go from there.

I want to keep Jekyll Now as minimal as possible. Every line of code should be one that's useful to 90% of the people using it. Please bear that in mind when submitting feature requests. If it's not something that most people will use, it probably won't get merged. :guardsman:
