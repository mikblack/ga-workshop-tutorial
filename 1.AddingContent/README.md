## Adding content to your workshop

Once the GitHUb repository has been setup with `README.md` and `LICENSE` files, it is time to add some content.

### Organisation of files

To keep things organised, a good approach is to use numbered folders.  As an example, the repository for this workshop contains four subdirectories:

 - 0.GettingStarted
 - 1.AddingContent
 - 2.ContentCreationExample
 - 3.ExampleContent

Within each directory is a another `README.md` file, each of which contains the material for that section of the course. Using this approaches means that as soon as a user navigates to that folder on GitHub, they will see the rendered markdown file for that section of the workshop.

There is also a directory called `images` within each folder, which contain any images that are linked from the `README.md` files.

The tree below provides an example of this style of layout:

```
├── 0.GettingStarted
│   ├── README.md
│   └── images
│       ├── create_repo.png
│       ├── edit_readme.png
│       ├── gh_updated.png
│       ├── new_repo.png
│       ├── rendered_readme.png
│       ├── vs_add_folders_files.png
│       ├── vs_clone_repo_1.png
│       ├── vs_clone_repo_2.png
│       ├── vs_clone_repo_3.png
│       ├── vs_commit.png
│       ├── vs_edit_readme.png
│       ├── vs_extensions.png
│       ├── vs_gh_extension.png
│       ├── vs_md_colour.png
│       ├── vs_md_extension_1.png
│       ├── vs_md_extension_2.png
│       └── vs_preview_mode.png
├── 1.AddingContent
│   └── README.md
├── LICENSE
└── README.md
```

### Formatting

Markdown provides a wide range of formatting options. In this workshop, we try to keep things fairly simple:

The are a number of ways to add images into a Markdown document.  For example, this syntax:

```
![images/smiley.png]
```

will display a smiley emoji that is stored in the `images` subdirectory.

![](images/smiley.png)

One problem with this approach, however, is that it doesn't allow you to rescale the size of the image.

An alternative is to use the `<img>` tag. For example, this code:

```
<img width="20%" src="images/smiley.png">
```

will display the same image, scaling it down by 10% (note that only specifying either width or height will preserve the aspect ratio).

<img width="10%" src="images/smiley.png">

The examples above make use of "code blocks".  These can be created by placing a series of three tickmarks (```) above and below the text that forms the code block. For example, the syntax

\`\`\`<BR>
This is a block of code<BR>
\`\`\`

will produce the following output:

```
This is a block of code
```

It can also be useful to highlight file or folder names using monospace font.  To do this, use single tickmarks around the text to be highlighted.  For example, this sytax,

```
`These words` will be printed  in monospace
```

will produce:

`These words` will be printed  in monospace

Links can be added via the following syntax:

```
[text](file.html)
```

For example, this code:

```
[Genomics Aotearoa web site](https://www.genomics-aotearoa.org.nz/)
```

adds a link to the Genomics Aotearoa website:

[Genomics Aotearoa web site](https://www.genomics-aotearoa.org.nz/)

### What additional content is required?

 - data files (on Github or externally linked?)
 - software requirements (plus versions used)
 - code to be run

<font color="orange">Work in progress...</font>

### NeSI-specific points

<font color="orange">Work in progress...</font>

### Additional considerations
 
Ability to run workshop locally (i.e. not on NeSI systems)

- can a html link be created to the data files on teh NeSI filesystem that are being used for the workshop
- that would allow non-NeSI users to download the exact files being used, without any need to duplicate (and remember to update them) externally (e.g., on FigShare).

<font color="orange">Work in progress...</font>

Next step: [Content Creation Example](https://github.com/mikblack/ga-workshop-tutorial/tree/main/2.ContentCreationExample)