The default shell is fish, start bash.

Make changes to the code using vim.

To run the site:

jekyll serve

To build the site:

rm -rf _site
jekyll build

The above command will create a folder called _site. Copy the contents of this folder to your webspace.

scp -r _site nagpal@login.math.wisc.edu:/path_to_your_target_directory/
scp -r _site nagpal@login.math.wisc.edu:~            (this will copy to your home directory)


To see the website:

http://95.85.61.4:4000/


In the worst case scenario (if scp doesn't work), you will have to push the changes to github:

git add --all
git commit -m "some message"
git push

Then download the zipped file from https://github.com/aerohit/nagpalsite

Extract it, and then copy the _site directory.
