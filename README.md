# personal notes template

To scaffold the template into the current directory, use:

```sh
curl -L https://github.com/Gravitonic/gravy-notes-template/archive/refs/heads/main.zip | tar -xv --strip-components=1
```

## known issues

Subfiles using `minted` may not work properly with LaTeX Workshop for VS Code, since by default it produces minted cache files in the root directory, but compiling each subfile expects a minted cache directory in the directory of the subfile. Adding a `.latexmkrc` file in the root directory with `$do_cd = 1;` as recommended by LaTeX Workshop should work (see [here](https://github.com/James-Yu/LaTeX-Workshop/wiki/Compile#the-root-file)).
