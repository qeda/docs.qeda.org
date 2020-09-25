# Commands

You can see available commands when running QEDA CLI with `--help` option:

```bash
qeda --help
```

|               Command                |                                                              Description                                                              |                 Example                 |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| <nobr>[add](#add) *COMPONENT*</nobr> | Add a component entry to the configuration file (with preloading from the [remote repository](http://github.com/qeda/lib/) if needed) | <nobr>`qeda add capacitor/c0603`</nobr> |

## `add`

Firstly this command looks for _COMPONENT_'s YAML-description in `qedalib` directory (relatively to the current working directory). In case of its absence the command tries to download a component's description from the [remote repository](http://github.com/qeda/lib/). If the download is successful, this leads to caching this description file to the `qedalib` directory, the to add a corresponding entry to the `.qeda.yaml` configuration file. When called for the second time, the command will use the cached file instead of loading it from the remote repository.

If neither the local `qedalib` directory nor the remote repository contains the corresponding component description, the command will return the error.

**See also**: [load](#load)

