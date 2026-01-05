# plist.libsonnet

> This repo contains Jsonnet code for working w/ plists

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Dependencies](#dependencies)
- [Including in a Jsonnet project](#including-in-a-jsonnet-project)
  - [Using git submodules](#using-git-submodules)
- [Credits](#credits)
- [License](#license)
- [Contributing](#contributing)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Dependencies

You will need the following

- [jsonnet](https://jsonnet.org/)
- [task](https://taskfile.dev/) `Optional, makes working w/ Jsonnet easier`

## Including in a Jsonnet project

### Using git submodules

First you need to add this as a submodule to your git repo:

```sh
git submodule add https://github.com/s0cks/plist.libsonnet.git
```

Then you will need to include this using the `-J` flag when running Jsonnet:

```sh
# ex:
jsonnet \
    -J plist.libsonnet/ \
    ....
```

Now you can import this in your Jsonnet projects like such:

```libsonnet
// import the lib:
local plist = import 'lib/plist.libsonnet';
....
```

## Credits

TBD

## License

See [LICENSE](LICENSE)

## Contributing

See [Contributing](Contributing.md)
