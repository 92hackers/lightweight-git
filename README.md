# A lightweight git alike Version Control System

**Git** is so weight on some cases, such as:

There are many config files on server, often you will want to modify the config file
to see if everythings works, or debug why it's 500, in old way, you maybe create a `config-backup` file to
backup current file content, but, with such operations more and morr frequently, everything will be messed.
it's important to put server config files under a **VCS**.
but **git** is too complicated to such case, to store a file change, you will have to run below commands:

```bash
git add .
git commit -m "add: xxxxx"
```

In general, **git** desinged to be used in a serious way, you make sure what you did
and then store the updates.
but in some cases, you just want to modify something, save and see what happend, besides,
it's a important file.

That's why **lightweight-git** comes.

## Features

1. Auto commit changes when you save file content.
2. Support set up commit template.
3. Support squash commits by day, week, month.
4. Seamless migrate to git, when you want to push commits to a remote service,
  such as `github`.
5. Support almost all operations like git, such as checkout to a specific commit.
