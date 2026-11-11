# A Question for Prince

A single-page interactive proposal. No build step and no dependencies: the whole site is `index.html`.

## Deploy on GitHub Pages

1. Create a new repository on GitHub (public, any name, for example `for-prince`).
2. Upload `index.html` and `README.md` to the repository root (Add file, then Upload files, then Commit).
3. Open the repository's **Settings**, then **Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the `main` branch and the `/ (root)` folder, then **Save**.
5. Wait a minute or two. The site appears at `https://YOUR-USERNAME.github.io/for-prince/`.

### Using git instead

```bash
git init
git add index.html README.md
git commit -m "Add proposal page"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/for-prince.git
git push -u origin main
```

Then follow steps 3 to 5 above.

## Add your own song

1. Rename your audio file to `song.mp3` (`song.m4a`, `song.ogg` and `song.wav` also work).
2. Create a folder named `music` in the repository, next to `index.html`, and put the file inside it, so the path is `music/song.mp3`.
3. On GitHub's website, on a computer, drag the whole `music` folder into Add file, then Upload files, and commit. Or use git: `git add music/song.mp3`, `git commit` and `git push`.

The page plays that file on a loop. If no music file is found, it plays a built-in melody instead. Keep the file under about 10 MB so it loads quickly on a phone (GitHub's web upload limit is 25 MB per file).

## Notes

- Browsers only allow sound after a tap, so the music starts when she presses Continue. The Music button in the top corner turns it off and on.
- The fonts load from Google Fonts, so the page needs an internet connection to look its best.
- A public GitHub Pages link can be opened by anyone who has it, so send it only to Prince.
