tumblr-disqus-socialNews
========================

Disqus and tumblr small hack to turn the combination into a Social News experiment

Todo

* how to have a clean mobile theme
* responsive as fuck
* burger navigation menu
* credits

Specificities

* simple and minimal design
* simple and minimum configuration
	
Requirements

* active account on tumblr
* active account on disqus
* ability to follow a tutorial and read basic html code


# Step 1 - creating Tumblr blog

## Copy paste the template

Go to [Tumblr](https://tumblr.com) and create a new blog.

Go to the customize page <http://www.tumblr.com/customize/your-blog-name> of the newly created tumblr blog, then copy/paste all the code from this project's index.html by clicking on **Edit HTML**. You have to replace all the existing code - yes top to bottom includind <html> tags.

Save.

## Customize your template

Still on the customize page <http://www.tumblr.com/customize/your-blog-name>, fill those fields following your will:

* **Title**
* **Description**
* **Disqus Shortname** - how to get one is explained at step 2

# Step 2 - Disqus integration


1. Go to [Disqus](https://disqus.com/) and log in your account.
Go to [Dashboard](https://disqus.com/dashboard) page, and next to **Your Sites**, click on **+ Add**

* **Site URL**: your name-of-site.tumblr.com
* **Site Name**: name-of-site
* **Site Shortname**: whatever you feel like, personnaly i use the name of the tumblr. You will need to use this **Shortname** at next step
* **Enable Promoted Discovery**: do you want adverts?
	
2. The next step is on the setup page, and the only thing you have to do is again go back to your customize page on Tumblr <http://www.tumblr.com/customize/your-blog-name> and fill the field:

* **Disqus Shortname** - add your Disqus Shortname in this field
	
Now your main configuration is done.

Still, we need to complete one last step to be done, create or sections and navigation menu. Don't get scarred, this is as simple as licking an ice cream on a sunny sand/palmtree beach.

# Step 3 - Final step, get Sections and Navigation menu

Again, go to the customize page on Tumblr <http://www.tumblr.com/customize/your-blog-name>.

Reach the **Pages** section and click on add page.

* Select **Standard Layout**, you will use this template project and everything will work flowy. 
* **Page URL**: it will be your-blog-name.tumblr.com/pageURL
* **Page Titl**e: will apear in your navigation menu and on the home page
* **Show a link to this page**: `YES!` It is ultra important, otherwise you won't have your navigation displayed.
* Click **Save** for each page (on the configuration popup), of course.
* Click **Save** again, on the tumblr template

Your Tumble/Disqus Social News Group is now ready to be used.

# Other configuration

* You can of course add a **custom domain name** by going to [Tumblr configuration page](https://www.tumblr.com/settings). Eventually nothing will be broken.
* On <http://disqus-short-name.disqus.com/admin/settings/advanced> , so Disqus > Settings > Advanced you can add **Trusted Domains** that will prevent the module to be added on an other site than the one you decide.
* You can **password protect** you Tumblr on the [Tumblr configuration page](https://www.tumblr.com/settings)

# Troubleshooting

## "We were unable to load Disqus"

If you get the message "*We were unable to load Disqus. If you are a moderator please see our troubleshooting guide*".

You should reach your customize page on Tumblr <http://www.tumblr.com/customize/your-blog-name>, click the `edit HTML` button, go to the bottom of the page and locate:

```
//
// Disqus username
//

var disqus_shortname = '{text:Disqus Shortname}';
```

Then, replace `{text:Disqus Shortname}` by your actual username.

The reason this code is here is to prevent users to go into the code and make the experience as easy as possible.
