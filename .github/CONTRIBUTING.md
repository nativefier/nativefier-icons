## Contributing

Feel free to submit a pull request for any `.ico`, `.icns` or `.png` icon!

- `.ico` - For Windows
- `.icns` - For OSX
- `.png` - For Linux

If the icons for the correct platforms are found here, the [optional dependencies](https://github.com/jiahaog/nativefier/#optional-dependencies) for Nativefier might not be required to infer an icon for that particular target web page.

### Naming Convention

Name the icon file to `${PRODUCT}.${EXT}`, just use the key identifier for the page.

However, if the product name is generic enough, name it as `${COMPANY}-${PRODUCT}.${EXT}`, with `-` as the delimiter. The matching algorithm works by taking a score of the number of words matched in the file name with the target url. 

Take the example of naming Google Photos for the target url `https://photos.google.com/`. Using `photos.png` is too generic, and we want it to be specific to google. Thus, we will name the icon file `google-photos.png` for a `.png` file. 

### Step 1

First prepare the image files, for the respective platform as stated above

A helpful tool for converting the icons is [iconverticons.com](https://iconverticons.com/online/).

Copy the images to `./files`.

```
$ ls -a ./files

google-photos.png
google-photos.ico
google-photos.icns
```

### Step 2

Add an entry for the file to `./data/gitCloud.yml`, in alphabetical order

```yml
- name: google-photos
  href: files/google-photos.png
- name: google-photos
  href: files/google-photos.ico
- name: google-photos
  href: files/google-photos.icns
```

### Step 3

You're done! Submit a pull request with the changes and I'll merge them in as soon as possible.
