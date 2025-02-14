# FiftyOne Plugins 🔌🚀

A curated collection of
[FiftyOne Plugins](https://docs.voxel51.com/plugins/index.html), organized into
the following categories:

-   [Core Plugins](#core-plugins): core functionality that all FiftyOne users
    will likely want to install. These plugins are maintained by the FiftyOne
    team
-   [Voxel51 Plugins](#voxel51-plugins): non-core plugins that are officially
    maintained by the FiftyOne team
-   [Example Plugins](#example-plugins): these plugins exist to inspire and
    educate you to create your own plugins! Each emphasizes a different aspect
    of the plugin system
-   [Community Plugins](#community-plugins): third-party plugins that are
    contributed and maintained by the community. These plugins are not
    officially supported by the FiftyOne team, but they're likely awesome!

🔌🤝 **Contribute Your Own Plugin** 🚀🚀

Want to showcase your own plugin here? See the
[contributing section](#contributing) for instructions!

## Core Plugins

<table>
    <tr>
        <th>Name</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><b><a href="https://github.com/voxel51/fiftyone-plugins/blob/main/plugins/io/README.md">@voxel51/io</a></b></td>
        <td>📁 A collection of import/export utilities</td>
    </tr>
</table>

## Voxel51 Plugins

<table>
    <tr>
        <th>Name</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><b><a href="https://github.com/voxel51/voxelgpt">@voxel51/voxelgpt</a></b></td>
        <td>🤖 An AI assistant that can query visual datasets, search the FiftyOne docs, and answer general computer vision questions</td>
    </tr>
</table>

## Example Plugins

<table>
    <tr>
        <th>Name</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><b><a href="https://github.com/voxel51/fiftyone-plugins/blob/main/plugins/hello-world">@voxel51/hello-world</a></b></td>
        <td>👋 An example of JavaScript and Python components and operators in a single plugin</td>
    </tr>
        <tr>
        <td><b><a href="https://github.com/voxel51/fiftyone-plugins/blob/main/plugins/python-view/README.md">@voxel51/python-view</a></b></td>
        <td>🔎 Create views in the FiftyOne App with Python</td>
    </tr>
    <tr>
        <td><b><a href="https://github.com/voxel51/fiftyone-plugins/blob/main/plugins/examples/">@voxel51/examples</a></b></td>
        <td>📋 Examples of how to use the operator type system to build custom FiftyOne operations</td>
    </tr>
    
</table>

## Community Plugins

🔌🤝 **Contribute Your Own Plugin** 🚀🚀

Want to showcase your own plugin here? See the
[contributing section](#contributing) for instructions!

<table>
    <tr>
        <th>Name</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><b><a href="https://github.com/jacobmarks/image-quality-issues">@jacobmarks/image_issues</a></b></td>
        <td>🌩️ Find common image quality issues in your datasets</td>
    </tr>
    <tr>
        <td><b><a href="https://github.com/jacobmarks/concept-interpolation">@jacobmarks/concept_interpolation</a></b></td>
        <td>📈 Find images that best interpolate between two text-based extremes!</td>
    </tr>
    <tr>
        <td><b><a href="https://github.com/jacobmarks/ai-art-gallery">@jacobmarks/ai_art_gallery</a></b></td>
        <td>🎨 Create your own AI Art Gallery with Text-to-image models and FiftyOne!</td>
    </tr>
</table>

## Using Plugins

### Install FiftyOne

If you haven't already, install
[FiftyOne](https://github.com/voxel51/fiftyone):

```shell
pip install fiftyone
```

### Installing a plugin

In general, you can install all plugin(s) in a GitHub repository by running:

```shell
fiftyone plugins download https://github.com/path/to/repo
```

For instance, to install all plugins in this repository, you can run:

```shell
fiftyone plugins download https://github.com/voxel51/fiftyone-plugins
```

You can also install a specific plugin using the `--plugin-names` flag:

```shell
fiftyone plugins download \
    https://github.com/voxel51/fiftyone-plugins \
    --plugin-names <name>
```

**💡 Pro tip:** Some plugins require additional setup. Click the plugin's link
and navigate to the project's README for instructions.

### Plugin management

You can use the
[CLI commands](https://docs.voxel51.com/cli/index.html#fiftyone-plugins) below
to manage your downloaded plugins:

```shell
# List all plugins you've downloaded
fiftyone plugins list

# List the available operators
fiftyone operators list

# Disable a particular plugin
fiftyone plugins disable <name>

# Enable a particular plugin
fiftyone plugins enable <name>
```

### Local development

If you plan to develop plugins locally, you can clone the repository and
symlink it into your FiftyOne plugins directory like so:

```shell
cd /path/to/fiftyone-plugins
ln -s "$(pwd)" "$(fiftyone config plugins_dir)/fiftyone-plugins"
```

## Contributing

### Showcasing your plugin 🤝

Have a plugin you'd like to share with the community? Awesome! 🎉🎉🎉

Just follow these steps to add your plugin to this repository:

1.  Make sure your plugin repo has a `README.md` file that describes the plugin
    and how to install it
2.  Fork this repository
3.  Add an entry for your plugin to the [Community Plugins](#community-plugins)
    table above
4.  Submit a pull request into this repository

### Contributing to this repository 🙌

You're also welcome to contribue to the plugins that live natively in this
repository. Check out the [contributions guide](CONTRIBUTING.md) for
instructions.

## Join the Community

If you want join a fast-growing community of engineers, researchers, and
practitioners who love computer vision, join the
[FiftyOne Slack community](https://slack.voxel51.com/) 🚀🚀🚀

**💡 Pro tip:** the `#plugins` channel is a great place to discuss plugins!

## About FiftyOne

If you've made it this far, we'd greatly appreciate if you'd take a moment to
check out [FiftyOne](https://github.com/voxel51/fiftyone) and give us a star!

FiftyOne is an open source library for building high-quality datasets and
computer vision models. It's the engine that powers this project.

Thanks for visiting! 😊
