<div align="right">
   <a href="README_CN.md">中文</a> | <strong>English</strong>
</div>

<img src="https://cdn.fosstodon.org/accounts/avatars/111/137/925/464/599/407/original/5a723b0c04db75a8.png" alt="Hugo logo" width="100" height="100" align="right" />

<div align="center">

<h1> Hugo Template </h1>

<p>A fast and flexible static site generator built with love by bep, spf13, and friends in <a href="https://go.dev/">Go</a>.</p>

</div>

<hr/>

<div align="center">
<a href="https://themes.gohugo.io">Demo</a> | 
<a href="https://gohugo.io">Official</a> | 
<a href="https://gohugo.io/documentation/">Docs</a> | 
<a href="https://discourse.gohugo.io">Community</a>
</div>

<hr/>

## Get Started

### Define Domain

Change the `baseURL` in `config.yml` to your site's URL

```yml
baseURL: "https://lopins.github.io/hexo-template"
```

or 

```toml
baseURL= "https://lopins.github.io/hugo-template"
```

### [Configure Theme](https://github.com/lopins/hugo-template/issues/2)

1. pull theme into `themes/` and update it.

   `git submodule add git@github.com:adityatelange/hugo-PaperMod.git themes/hugo-PaperMod && git submodule update --init --recursive`

2. update `theme: "hugo-PaperMod"` in `config.yml` and configure other fields

3. update `editPost: "https://github.com/lopins/hugo-template/tree/main/content"` in `config.yml` 

4. into  `themes/hugo-PaperMod` to configure the theme in `theme.yml`

### Push to Github

`git add . && git commit -m ':wrench:docs(themes): Add or update configuration files' && git push origin main`

### [Publish Article](https://github.com/lopins/hugo-template/issues/1)

1. Install

   Click "Use this template" -> "Create a new repository"

![1. Create a new repository](https://github.com/user-attachments/assets/1046f118-8c2a-4ed8-bc8b-1258941455c4)

2. Set up

   Set up and enable GitHub Pages service

![2. Set up GitHub Pages branch](https://github.com/user-attachments/assets/acd90bfd-0a25-4809-a39b-fc5d562f414b)

3. Publish

   Publish an article on the "hugo branch" of Github.

![3. Write or Upload an Markdown file](https://github.com/user-attachments/assets/2b1a97ea-ac79-4647-a340-f71569699c11)

## Notice

### **Submodule** to Change Theme

```
# Add Submodule - Upadte Submodule
git submodule add git@github.com:adityatelange/hugo-PaperMod.git themes/hugo-PaperMod
git submodule update --init --recursive

# Delete Submodule
git submodule deinit -f themes/hugo-PaperMod
rm -rf .git/modules/themes/hugo-PaperMod
rm -rf themes/hugo-PaperMod

# Display Submodule - Pull Submodule - Sync Submodule
git submodule status
git submodule foreach git pull origin main
git submodule sync
```

### Permission

If you meet the problem like `remote: Permission to xxx denied to github-actions[bot].` 

When you push your changes, you need to give the permission to the `github-actions[bot]` in your repo's.

By following the steps below: `Settings -> Actions -> General -> Workflow permissions -> Read and write permissions -> Save`.

## License

[MIT License](LICENSE).