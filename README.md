# Converting app notes from docx to markdown

1. Find a .docx file in the app-notes repo (or somewhere - one that includes images and some applied styles)

2. Install pandoc

`brew install pandoc`

3. Do a pandoc

`pandoc --extract-media ./myMediaFolder -f docx -t gfm -o appnote-test.md apnt_xxx.docx`

Use `gfm` (Github flavoured markup) output to avoid weird thing with image positioning being rendered in markdown.
`--extrac-media` pulls out images etc and drops them in to a directory that will be referenced by the `.md` file.


