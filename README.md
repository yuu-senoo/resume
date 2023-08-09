# resume

## Features

### 💅 Lint text

Automatic proofreading with [textlint](https://github.com/textlint/textlint).

```
$ yarn lint --fix
```

It is also automatically executed when pre-commit by [husky](https://github.com/typicode/husky).  
proofreading rules are set with `.textlintrc`.

### 📝 Convert MD to PDF

You can generate PDF with [md-to-pdf](https://www.npmjs.com/package/md-to-pdf).

```
$ yarn build:pdf
```

The output PDF can be styled as you like with CSS. Edit the `pdf-configs/style.css`.

### 🛠 Create release

When you push with a `v**` tag, GitHub Actions will run the build, generate the PDF, create a Release, and register the PDF to Assets.

```
$ git commit -m "add job"
$ git tag v1.0
$ git push origin --tags
```
