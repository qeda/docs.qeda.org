# Commands

You can see available commands when running QEDA CLI with `--help` option:

```bash
qeda --help
```

|               Command                |                                                              Description                                                              |                 Example                 |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| <nobr>[add](#add) *COMPONENT*</nobr> | Add a component entry to the configuration file (with preloading from the [remote repository](http://github.com/qeda/lib/) if needed) | <nobr>`qeda add capacitor/c0603`</nobr> |
| <nobr>[config](#config) *PARAM* \[*VALUE*\]</nobr> | Set/get configuration parameter (see [Configuration Parameters](/cli/configuration.html)) | <nobr>`qeda config generator.type kicad`</nobr> |
| <nobr>[generate](#generate) *LIB* </nobr> | Generate a library for specified EDA according to the configuration file | <nobr>`qeda generate mylib`</nobr> |
| <nobr>[load](#load) *COMPONENT*</nobr> | Load a component description from the [remote repository](http://github.com/qeda/lib/) | <nobr>`qeda load capacitor/c0603`</nobr> |

## `add`

Firstly this command looks for _COMPONENT_'s YAML-description in the `qedalib` directory (relatively to the current working directory). In case of its absence the command tries to download a component description from the [remote repository](http://github.com/qeda/lib/). If the download is successful, this leads to caching this description file to the `qedalib` directory, the to add a corresponding entry to the `.qeda.yaml` configuration file. When called for the second time, the command will use the cached file instead of loading it from the remote repository.

If neither the local `qedalib` directory nor the remote repository contains the corresponding component description, the command will return the error.

**See also**: [load](#load)

## `config`

This command allows to set or get a configuration parameter of the electronic component library to be generated. To set the *PARAM* you need to provide the *VALUE* as a second argument. To get the parameter value one should omit the *VALUE* argument.

See [Configuration Parameters](/cli/configuration.html) for full available parameters list.

## `generate`

The final command which generates a library of electronic components to be used in EDA according to the settings found in the `.qeda.yaml` configuration file.

## `load`

This command loads and caches a component description from the [remote repository](http://github.com/qeda/lib/) regardless of its presence in the `qedalib` directory **without** adding it to the `.qeda.yaml` configuration file.

**See also**: [add](#add)