# degit-sync

A helper tool for syncing local git repositories to remote machines.

This tool is designed to sync to machines which have to no access to the outside world besides SSH.
It uses rsync, but does not sync hidden files (like the .git directory) and toplevel `build` directories.

## Usage
Work on your project, make changes (commit them or not) and inside of the git project run

```sh
degit-sync push user@remote:path/to/synced/repo
```

Try to compile your project on the remote machine, cry in despair, fix the bug on the remote machine and run

```sh
degit-sync pull user@remote:path/to/synced/repo
```

on the local machine

Commit your changes in your local repository and wait until the next bug.

# License

This tool is licensed under MIT. See [LICENSE](LICENSE) for details.

Copyright 2022 Tim Niklas Uhl
