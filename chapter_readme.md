# README for Chapters

This document serves to both tell you about your new site and give you instructions on how to do anything you want to do with your site. All these instructions assume you have the Github repository open in a browser tab: [your chapter's repository](https://github.com/dsa-ntc/midmissouridsa-ntc.github.io).

If instructions are missing for something you want to do or if you have a question that this page doesn't answer, please reach out to the NTC for help. Doing so will allow us to add more information to this page, so other chapters can benefit.

## Site Features

### RSS Feed

In the footer at the bottom of every page there is a link to the site's RSS feed. This is updated automatically when you make a new blog post. Readers can subscribe to the RSS feed using an RSS reader, and be notified when you make a new post.

## Adding a New Post

Go to the `_posts` directory.

![Highlighting the _posts directory](/readme-assets/chapter_readme/posts-click.png)

Click the "Add file" dropdown and then click the "Create new file" option.

![Create new file option](/readme-assets/chapter_readme/new-post.png)

Add the front matter at the top of the file and the post content at the bottom. Jekyll has a documentation page on both [front matter](https://jekyllrb.com/docs/front-matter/) and [posts](https://jekyllrb.com/docs/posts/). You can also look at your previous posts for what should be included in the front matter and how to include links and pictures.

![Post front matter and content](/readme-assets/chapter_readme/post-sections.png)

Name your post following the convention of your other posts: `YEAR-MONTH-DAY-name-of-your-post.md` and click the "Commit changes..." button.

![Post name and commit button](/readme-assets/chapter_readme/post-name-and-commit.png)

On the "Commit changes" screen, you can change the "Commit message" and "Extended description" if you'd like (or leave it as is). Hit the "Commit changes" button at the bottom, and the post will be published to your site in the next 10 minutes.

### Draft Posts

If you want to save a post as a draft before publishing it to your site, you can save the post in the `_posts/_drafts/` directory. To do this, you add `_drafts/` to the beginning of the filename in "Name your file..." box when editing the file. This will add the `_drafts` directory to the file path.

#### Moving a Post into the Drafts Directory

Here is what the filename will look like when the post is in the `_posts` directory:

![Post in `_posts` directory](/readme-assets/chapter_readme/post-move-to-drafts-1.png)

With your cursor at the beginning of the post name, type "_drafts":

![Post almost in `_drafts` directory](/readme-assets/chapter_readme/post-move-to-drafts-2.png)

Type "/" and the post will be moved into the `_drafts/` directory:

![Post now in `_drafts` directory](/readme-assets/chapter_readme/post-move-to-drafts-3.png)

Finally, press the "Commit changes..." button on the right to save the movement of the file.

#### Publishing a Draft Post

When you are ready to publish a post in your `_drafts` directory, you do almost the reverse of above, you will edit the post and remove `_drafts/` from the filename.

Here is what the filename will look like when the post is in the `_drafts` directory:

![Post in `_drafts` directory](/readme-assets/chapter_readme/post-move-to-drafts-3.png)

With your cursor at the beginning of the post name, hit the "Backspace" key. This will move the "_drafts" layer of the filepath into the file name box:

![Post in `_posts` directory with "_drafts" in file name box](/readme-assets/chapter_readme/post-move-to-drafts-2.png)

Delete the "_drafts" at the beginning of the file name to restore the original post name:

![Post now in `_posts` directory](/readme-assets/chapter_readme/post-move-to-drafts-1.png)

Finally, press the "Commit changes..." button on the right to save the movement of the file.

## Editing an Existing Page

Navigate to any page in the repository that you wish to edit and click the "Edit this file" button.

![Edit this file button](/readme-assets/chapter_readme/edit-this-file-button.png)

Make whatever changes you desire and clicke the "commit changes..." button.

![Post name and commit button](/readme-assets/chapter_readme/post-name-and-commit.png)

On the "Commit changes" screen, you can change the "Commit message" and "Extended description" if you'd like (or leave it as is). Hit the "Commit changes" button at the bottom, and the post will be published to your site in the next 10 minutes.

## Editing Landing Page Content

The file `_data/copy.yml` contains some of the text that shows up on your landing page, and some that shows up on every page. The `welcome` and `landing-page-text` show up on the landing page. The `about` is displayed in the footer of every page. Below are screenshots of the file itself and where the text appears on the landing page.

![The `_data/copy.yml` file](/readme-assets/chapter_readme/copy-file.png)

![The landing page with copy highlighted](/readme-assets/chapter_readme/copy-page-screenshot.png)

Edit this page as explained in the [Editing an Existing Page](#editing-an-existing-page) section. Your changes should be reflected on your site within 10 minutes.

## Editing the Navigation Header

The file `_data/nav.yml` determines which links appear in the header of every page.

![The nav header file](/readme-assets/chapter_readme/nav-header-file.png)

![Screenshot of the nav bar](/readme-assets/chapter_readme/nav-header-screenshot.png)

You can add or remove entries in the yml file to add or remove the links that appear in the navigation header.

One word of caution, adding too many links will cause the links to collide with the site title.

## Changing the Site Title

To change the site title, change the `title:` entry in the `_config.yml` file. This title appears in the navigation bar header, the footer of every page, and the tab text on the landing page.

## Changing the Site Icon

The logo shown at the top left of every page and at the bottom center of every page can be changed by changing the file specified in the `logo:` option in the `_config.yml` file found in the base directory of your repository.

You will have to upload the image file first. Navigate to the `assest/images/` folder on GitHub, click the "Add file" dropdown menu, and select "Upload files":

!["Upload files" button](/readme-assets/chapter_readme/upload-files.png)

## Adding a New Non-Post Page

To add a new non-post page to the site, navigate to the `_pages` folder.

![Base folder with `_pages` directory highlighted](/readme-assets/chapter_readme/pages-click.png)

Click the "Add file" dropdown and then click the "Create new file" option.

![Create new file option](/readme-assets/chapter_readme/new-page.png)

Add the front matter at the top of the file and the page content at the bottom. Jekyll has a documentation page on both [front matter](https://jekyllrb.com/docs/front-matter/) and [posts](https://jekyllrb.com/docs/posts/). You can also look at other pages for what should be included in the front matter and how to include links and pictures.

![Page front matter and content](/readme-assets/chapter_readme/page-sections.png)

Give your page a name and click the "Commit changes..." button.

On the "Commit changes" screen, you can change the "Commit message" and "Extended description" if you'd like (or leave it as is). Hit the "Commit changes" button at the bottom, and the post will be published to your site in the next 10 minutes.

After the page has been created you will need some way for users to get to the page. You can use your new page's url in any of your existing pages or a post:

Inserting `[New Page Title](/_pages/new-page-title/)` will create a link to your new page.

You can also add the page to the navigation bar that appears at the top of every page. See [Editing the Navigation Header](#editing-the-navigation-header) for instructions.

## Adding Pictures to Pages and Posts

Pictures can be inserted into posts an non-post pages. The syntax for adding pictures to markdown files can be found [here](https://www.markdownguide.org/basic-syntax#images-1). Additionally, you can look at the raw markdown for this page to see several examples. The one convention Jekyll follows is that you put the images in the `assets/images/` folder.

Adding images to the repository is done similarly to how you create a new post. Navigate to the `assest/images/` folder on GitHub, click the "Add file" dropdown menu, and select "Upload files":

!["Upload files" button](/readme-assets/chapter_readme/upload-files.png)

## Specifying Social Media Accounts

`_data/social.yml` contains the social media accounts you want shown on your page. The top half of the page is where you provide the information for the social media accounts you have. The bottom half states which social media accounts are shown on various parts of pages.

![Social Media Accounts](/readme-assets/chapter_readme/social-media.png)

You can comment or uncomment the lines in the file (put a '#' at the beginning of the line to comment out (it won't be read by the site generator) the line) to control whether the social media account is shown on the various parts of your site.

If there is a social media account that you have that we don't have in the file, let the NTC know so we can add it to the template.

## Useful Reference Links

* Github documentation on creating, editing, moving, and deleting files: <https://docs.github.com/en/repositories/working-with-files/managing-files>
* Jekyll documentation on posts: <https://jekyllrb.com/docs/posts/>
* Jekyll documentation on front matter: <https://jekyllrb.com/docs/front-matter/>
* Markdown documentation: <https://www.markdownguide.org/basic-syntax/>
