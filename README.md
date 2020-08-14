# Docker-tinytex-make

`tinytex-base.docker` provides a base install of tinytex on Ubuntu focal, since using Alpine [might not be possible](https://tex.stackexchange.com/questions/493664/).

## Customize the latex install

In order to install additional tex packages, use

```bash
tlmgr install <package name>
```

If you need to find out which package you are missing, from the missing file error
message, search which package the missing file belongs to using:

```bash
tlmgr search --global --file "/environ.sty"
```

## Awesome-CV image

`Awesome-CV.docker` provides a few additional packages that are required in order to generate an [Awesome-CV](https://github.com/gcuendet/Awesome-CV)
