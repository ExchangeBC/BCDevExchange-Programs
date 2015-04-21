# BCDevExchange-Programs
A repository for Programs, referenced by BCDevExchange.org

# Administration

## Directory
As an admin of this repo, you can add/edit the `directory.yml` file.  You may also allow others to fork it and you may accept pull requests.  

`directory.yml` is a list of programs as they will appear on [bcdevexchange.org/#/programs](https://bcdevexchange.org/#/programs).  The server will read the file from GitHub, parse the YAML and display the content.  

In the event the YAML has a parsing error, check the server logs `log/stderr.log` for details on the problem. If you run into a lot of problems with YAML, I suggest creating a branch or fork it while you work through the issues.  Then once validated, merge back to master via pull request.  

A helpful tool for validating the syntax:

[yaml-online-parser.appspot.com](http://yaml-online-parser.appspot.com/?url=https%3A%2F%2Fraw.githubusercontent.com%2FBCDevExchange%2FBCDevExchange-Programs%2Fmaster%2Fdirectory.yml)

Any logos referenced in the `directory.yml` should go into the `/Logo/` folder.  Logos will be presented as-is and therefore should be re-sized to an appropriate size.

## Program Pages
We encourage program owners or their delegates to provide content for program pages.  

Markdown files placed in the folder `/Programs/`.  The BCDevExchange app read the file, converts it to HTML, and then applies bootstrap CSS styles on it.  So it should look good and be responsive without any effort from the author.  

We support the following most vanilla markdown:

- Header 1-6
- Paragraph
- bold, italics, strike-through, mono-space text
- bullet lists, nested lists, numbered lists
- images (SHOULD use HTTPS)
- links
- Blockquotes
- Code blocks

Unsupported markdown (GitHub flavoured):

- Tables
- Emoji
- Auto linking
- @people

Extended markdown for layout purposes:

- [row start]
	 - This declares that a row is being created. Page will automatically define the spacing for 2 columns or 3 columns on the page, based on the number of columns that follow. 
- [col start] 
	- This declares the start of a distinct column. Any Titles or Content that follow will be displayed constrained by the column width. It is recommended that no more than 3 columns be displayed in a single row (this is a style recommendation, the technical limitation is 12).  
- [col end]
	- Declares the end of a distinct column. Subsequent [col start] can be declared.
- [row end]
	- Declares the end of a distinct row. Unless another row is declared, subsequent content will display in full page width.

*Note: row and col are converted to the bootstrap grid system.  Therefore, the col will stack on top of each other when forced to shrink on a smaller display.*

**See our [sample page](https://bcdevexchange.org/#/programs/Test%20title) of how styles are rendered.**


## Publishing and Previewing
While something is in draft you may not want to have it appear in the [program directory](https://bcdevexchange.org/#/programs).  Use the `visible` attribute in the program page listing in the `directory.yml` file.  Use the value, `no` to hide it.  When you're ready to make it visible, change the value `yes`. 

You may want to preview what the program page appears like before making it visible.  You can specially craft a URL to preview the page.  Take the title of the program (as entered in `directory.yml`) and add it to this URL:

```
https://bcdevexchange.org/#/programs/<title of program>
```

For example:

```
https://bcdevexchange.org/#/programs/Hidden%20Project
```

*Note the URL encoding of the space (%20) above.  Browsers automatically do this for you when you're typing in the URL bar and hit enter.*