# BCDevExchange-Programs
A repository for Programs, referenced by BCDevExchange.org

# Administration

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