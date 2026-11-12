# Björk website — GitHub Pages files

This folder contains the corrected website and its original images. No build or installation is needed.

## What caused the formatting problem

The original HTML requested stylesheets such as `Css/style.css` and photos such as `Images/black_and_white.jpeg`. In the GitHub repository, those files were uploaded directly beside `index.html`, so the requested folder paths did not exist. The HTML loaded, but the styles and photos did not.

The corrected files use relative paths to the files in the same folder. All five pages also use the correct `viewport` setting, and the CSS now keeps navigation, photos, videos and long reference links within smaller screens. The original wallpaper background is included as `background.jpeg`.

## Upload the corrected site

1. Unzip `bjork-github-fixed.zip` on your computer.
2. Open your `carsonguise/bjork` repository on GitHub and select the branch used for GitHub Pages.
3. From the repository's main file list, choose **Add file → Upload files**.
4. Open the extracted folder and select **all the files inside it**. Upload them directly beside the existing `index.html`. Include the HTML, CSS and JPEG files. Keep every file in the same folder.
5. Commit the changes. Files with the same names and paths replace the existing versions.
6. In **Settings → Pages**, confirm that the publishing source points to the branch you just updated. For a simple setup, use **Deploy from a branch → main → /(root)**. If your existing site uses a different branch, update that branch instead.
7. Check the repository's **Actions** tab for the Pages deployment to finish, then visit https://carsonguise.github.io/bjork/.
8. If the old version is still showing, use **Command + Shift + R** on Mac or **Ctrl + Shift + R** on Windows/Linux.

Upload the extracted files, not the ZIP itself or an extra folder containing the website. `index.html`, the five CSS files, and all JPEG images must be together at the publishing root.

## Files to keep together

- Pages: `index.html`, `history.html`, `discography.html`, `influences.html`, `references.html`
- Styles: `style.css`, `style_history.css`, `style_discrography.css`, `style_influences.css`, `style_references.css`
- Images: `background.jpeg`, `black_and_white.jpeg`, `bjork_history.jpeg`, `swan_dress.jpeg`, `debut.jpeg`, `post.jpeg`, `homogenic.jpeg`, `vespertine.jpeg`, `medulla.jpeg`, `volta.jpeg`, `biophilia.jpeg`, `vulnicura.jpeg`, `utopia.jpeg`, `fossora.jpeg`

The original spelling of `style_discrography.css` is retained so the upload replaces the existing filename. The corrected HTML links to that exact name.

## Validation

All five pages were checked in a desktop browser and at phone width. All local stylesheet, image and navigation paths resolve, and the pages fit the phone viewport without horizontal overflow. YouTube embeds still use the original external videos; one displayed an unavailable message during the preview.

GitHub Pages publishing documentation: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
