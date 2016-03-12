## Contributing

Feel free to submit a pull request for any `.ico`, `.icns` or `.png` icon!

- `.ico` - For Windows
- `.icns` - For OSX
- `.png` - For Linux

If the icons for the correct platforms are found here, the [optional dependencies](https://github.com/jiahaog/nativefier/#optional-dependencies) for Nativefier might not be required to infer an icon for that particular target web page.

For example, I want to add an `.ico` file to the repository, for [http://www.facebook.com/](http://www.facebook.com/).

### Naming Convention

Rename the icon file to `facebook.ico`, just use the key identifier for the page.

### Step 1

Copy the file to `./files`

### Step 2

Add an entry for the file to `./data/gitCloud.yml`

For example, add the following lines to the end of the file.

```yml
- href: files/facebook.ico
  name: facebook
```

### Step 3

You're done! Submit a pull request with the changes and I'll merge them in as soon as possible.
