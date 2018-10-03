# Sugarpops

Custom site builder and content of my travel blog 👉 [sugarpops.world](http://sugarpops.world)

## To make a new blog post

- Post copy `templates/post.post` file into the `source/` directory
- Rename the file with a the title of the post
- Write your post
- Place images in the `source/images/` directory
- Make the site to see the changes
- Deploy when happy with the result

## Tools

There are a few command line tools to work with:

    bin/make    Makes the site from files in source/ to public/ using templates in templates/
    bin/clean   Removes all files in public/
    bin/deploy  Deploys the site to server

There is also the `Resize-images.workflow` used resize images to 1200px width in batch. 

## Technical notes

### The hero image ratio is 2.4

    2.4 (width) / 1 (height)
    w = h * 2.4
    h = w / 2.4

or

    1600 x 666

### Cut images at 1280 x 800 pixel

Macbook screen size is 1280 by 800 so cut the images at that size.
