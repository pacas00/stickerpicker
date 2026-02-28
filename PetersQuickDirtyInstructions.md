This is a combination of the documentation from https://github.com/maunium/stickerpicker that can be referenced in one place.


you need FFMPEG and gifsicle.
Install FFMPEG is a package manager friendly way. Do the below for gifsicle.

```
curl -sL http://www.lcdf.org/gifsicle/gifsicle-1.91.tar.gz | tar -zx
cd gifsicle-1.91
./configure --disable-gifview
sudo make install
```

Prep

1. `git clone https://github.com/pacas00/stickerpicker.git`

2. CD into directory

3. Set up a virtual environment. (Because dont break package installed python3)
   Create with `virtualenv -p python3 .venv`
   Activate with `source .venv/bin/activate`

4. Install the utility commands and their dependencies with `pip install .`


5. Create a directory in emotes to store your new emotes in (or add to an existing folder)


6. Call sticker-pack FROM THE REPO ROOT with the folder path RELATIVE TO THE REPO ROOT and add to the index. see example below

`sticker-pack emotes/calculon_emotes --add-to-index web/packs`


7. Add, Commit and Push
`git add emotes/`
`git add web/packs/`

`git commit`

`git push`