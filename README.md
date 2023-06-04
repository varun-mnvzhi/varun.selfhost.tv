[//]: # (What this?)
# What is this?
Aesthetically minimal and light-weight video gallery website template
This template aims at automation and scalability for portfolio-like websites with ease-of-use. Consider, that you are an editor and you want to make a website without needing to code. Your options are wordpress, squarespace, notion, wix, etc. You will find yourself uploading videos one by one and placing each of them in an WYSIWYG online editor. I feel this is a repetitive process and demotivates young artists from maintaining their own website. I want automation in this process such that having more content doesnt mean more work, also when you want to change the theme of your website.

[//]: # (For who?)
# Is this for you?
Are you an actor? Maybe, you are a cinematographer or an editor. Perhaps you are a hobbyist web developer. This template is suitable for artists who want to show off videos. If you are a hobbyist web developer, you can tinker with Jekyll/HTML/CSS/JS.

[//]: # (How?)
# Get started
There are two ways to use this project: for artists and for hobbyist web developers. I am slowly updating the instructions and making them more detailed. Feel free to open an issue.

## Artists
NOTE: Git and GitHub terminology is not part of the instructions.
Artists can use this right away without any coding. You will obtain a copy of this repository, and learn to tweak. Please follow these steps:

### Get started (artists)
1. Make a GitHub account.
2. `Fork` this repository. Change the Repository name and description as appropriate.
3. Make sure copy the `main` branch only is selected. Click `Create fork` and you will have a copy of this template in your account.
4. Go to `Settings > Code and Automation: Pages` of the reposiory. Under `Build and deployment`, make sure the `Source` dropdown is set to `Deploy from a branch` and the `Branch` is set to `main`. Then, make sure that `/(root)` is selecetd in the second dropdown.
5. Make sure there is no custom domain set. Go to Section [Set a custom domain](#set-a-custom-domain).
6. You shall get a notification that a pages build and deployment workflow is running. This workflow will automatically build and deploy your forked copy as a website within minutes.
7. In a couple of mintes your forked copy should be live at `<USERNAME>.github.io/<REPOSITORY>`, e.g. this template is at [saumil-sh.github.io/varun.selfhost.tv](saumil-sh.github.io/varun.selfhost.tv).

### Personalizing the template
1. When you click on your repository name at the top in GitHub, you'll be redirected to the repository "homepage". Here, you'll see a file browser; find the file `_config.yml`, and click on it. The `.yml` is a human-readable configuration file containing website informaiton. You need to edit it only once at the time of setup. Change the `title` and `url` values to appropriate values. The `title` appears as the last part of the title in a tab of a web browser nex to favicon. If you are not using a custom domain, then `url` must be set to `<USERNAME>.github.io/<REPOSITORY>`. Respect the ` ` after `:` as `.yml` files are sensitive to this space.
2. Replace the `assets/img/logo.svg` and `assets/img/logo.svg` with your brand. Use `Add file` dropdown, located at the top, and select `Upload files`. This is a one-time change.
3. Go to `_includes/footer.html`, the `div` tag at line 5 holds information about social media. This is a one-time change. You can have entries of your choice there, consider following examples:
    ```html
    <a href="https://vimeo.com/<HANDLE>"><i class="fab fa-vimeo"></i></a>
    ```
    ```html
    <a href="mailto:EXAMPLE@EMAIL.COM"><i class="fab fa-paper-plane"></i></a>
    ```

### Adding new content
New parent pages are added to the `root` directory and child pages are added in `_pages`.
`index.md`, `about.md`, `parent-A.md`, and `parent-B.md` are parent pages and they appear in the navigation bar of the website. `child-A1.md`, `child-A2.md`, and `child-B1.md` are sub pages that appear in corresponding parent page, but do not appear in the navigation bar. This project converts markdown files with YAML front-matter into a website. The instructions on YAML front-matter are commented in the respective files.