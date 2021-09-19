# Conjure issue with Neovim nightly

A reproduction for an issue with Conjure and Neovim nightly.

## How to reproduce the issue

Execute the following Docker command:

```sh
docker build -t issue . && docker run -it issue
```

After that create a new Fennel file like:

```sh
nvim test.fnl
```

Write any valid Fennel expression like `(+ 1 2)` and try to evaluate it using
Conjure (e.g. using `<localleader>e`).

**Note:** `<localleader>` is mapped to `<space>`.

## Evidence

![image](https://user-images.githubusercontent.com/37723586/133939095-fbcbc39b-8d9c-4370-920d-ea31453c7bc0.png)
