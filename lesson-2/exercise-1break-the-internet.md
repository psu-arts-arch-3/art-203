### Requiremnets

Download and install[ Filezilla](https://filezilla-project.org/) \(FTP app\) and [Brackets](http://brackets.io/) \(rich text editor\).

### Create a local directory

Create a local directory on your computer; we'll create new files and edit them here before uploading them to the Web. Create a folder in your Documents folder or User folder called "local-directory" or "sites" \(without the quotes\) or whatever you want to call it \(remember—no spaces!\).

### Create an HTML file

1. Open Brackets 
2. File &gt;&gt;&gt; Open folder
3. Select your local directory. 
4. File &gt;&gt;&gt; New
5. Paste in the following code for a basic HTML document

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Page Title</title>
    </head>
    <body>
        <!-- Add content here -->

    </body>
</html>
```

Add some text below the "Add content here" comment; remember to wrap your text in `<p>` or `<h1>` tags.

For example: `<h1>Hello world!</h1>`

It's good practice to indent each line of text \(press tab\) to show levels of hierarchy—as seen below—but if you don't, the website will still work.

![](/assets/brackets-code.png)

File &gt;&gt;&gt; Save

Save this new file as "index.html"

![](/assets/brackets-save.png)

Now find your index.html file in your file browser, and double click on it to open it in a web browser. Nice job!

![](/assets/browser-hello.png)

## Setup FTP

Now open Filezilla. At the top of the window, there are fields labeled Host, Username, Password, and Port.

Enter the following information to direct the program to our virtual folder hosted through PSU.

* **Host: **sftp.pass.psu.edu
* **Username:** Your PSU username \(e.g. "jsmith123"\)
* **Password: **Your PSU password
* **Port:** 22

Click "Quickconnect" — you may get a warning message, but it's probably fine to just hit okay. PSU's servers may not match the ideal standards held by Filezilla's developers.

After a few seconds you should see some folders appear on the right side of the screen. If you get an error message, you may have typed something in wrong, or your PASS directory may not have been activated yet. If it's still not working, you can try using the in-browser file manager: [https://explorer.pass.psu.edu/](https://explorer.pass.psu.edu/)

The Filezilla interface is divided into two sections: your local directory \(left\) and your remote directory \(right\). You can drag files back and forth to upload or download.

![](/assets/filezilla-diagram.png)

You will have to navigate to your local directory on the left side until you can se the index.html file you created. Drag it into the "www" folder on the server to replace the existing "index.html" file.

Now see check that it uploaded successfully by going to: "[http://personal.psu.edu/user123](http://personal.psu.edu/user123)" — but replace "user123" with your PSU username.

While we're here, let's create a folder for storing our upcoming projects. 

### Create a new Directory

In Filezilla, right-click in the lefthand window and choose "Create directory" — you could also just create the folder in your regular file browser. 

Call the new folder "art203" \(without quotes\).

Upload the empty folder to your remote directory. 



**Submit your URL to the following assignment: **

\[INSERT ASSIGNMENT LINK\]

