# The Demo Project of WEB Language created by Knuth

## Prerequisite

Install `texlive` beforehand. `weave` and  `tangle` was included.
Install Pascal compiler.
```shell
brew install texlive
brew install fpc
```

### Source Code

```shell
example.web
```

## Generating Documentation

### Generating TEX file

```shell
weave example.web
#output file: example.tex
```

### Transform TEX to PDF

```shell
pdftex example.tex
#output file: example.pdf
```

## Generating Executable

### Generating the Pascal code
```shell
tangle example.web
#output file: example.p
```

### Compile the code
```shell
fpc example.web
#output binary: example
```

### Run it
```shell
./example
```