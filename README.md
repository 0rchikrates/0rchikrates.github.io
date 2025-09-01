# 0rchikrates.github.io
Simple Greek Text Viewer for GitHub Pages
This project displays Greek text from an XML file, converting it from Beta Code to Unicode on the fly.

How to Deploy to GitHub Pages
Follow these steps to get your own version of this website online for free.

Step 1: Create a GitHub Repository
Log in to your GitHub account.

Click the + icon in the top-right corner and select New repository.

Give your repository a name (e.g., greek-texts).

Make sure it's set to Public.

Click Create repository.

Step 2: Upload the Files
In your new repository, click the Add file button and choose Upload files.

Drag and drop the index.html and plato_text.xml files into the upload area.

Click Commit changes.

Step 3: Enable GitHub Pages
In your repository, go to the Settings tab.

In the left sidebar, click on Pages.

Under "Branch", select main (or master if that's your default branch) from the dropdown menu and leave the folder as /root.

Click Save.

Step 4: Visit Your New Site!
GitHub will now build and deploy your site. This can take a minute or two.

Once it's ready, a green bar will appear at the top of the Pages settings with a link to your live site. The URL will look something like this:

https://<your-username>.github.io/<your-repository-name>/

That's it! You now have a live website.

How to Use Your Own Text
To display your own text, simply replace the contents of plato_text.xml with your own XML file's content. Make sure the structure is similar, or be prepared to adjust the JavaScript in index.html to find the correct text elements.

Specifically, this line in the index.html file looks for the text:
const sections = xmlDoc.querySelectorAll('div[type="textpart"][subtype="section"]');

You may need to change the querySelectorAll value to match the tags in your XML file.
