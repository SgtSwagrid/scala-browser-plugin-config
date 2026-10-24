<div align="center">
  <h1>⚙️ Scala Browser Plugin Config</h1>
  <p>Common configuration for all of my Scala browser plugins.</p>
</div>

## 👷 What's the workflow?

Changes made to the configuration files contained herein are automatically copied into each dependent project using [GitHub Graph](https://github.com/SgtSwagrid/github-graph).
Updates to these files should be made _here_, not in any of the downstream repositories, lest they be overwritten later.

## 📋 What's included?

- Everything from [Scala Config](https://github.com/SgtSwagrid/scala-config).
- SBT plugins for building browser plugins with [Omnibrowser](https://github.com/SgtSwagrid/omnibrowser), which compiles them to JavaScript with [Scala.js](https://www.scala-js.org/) and lays them out for Chrome and Firefox, and for naming each version by its git tag with [sbt-dynver](https://github.com/sbt/sbt-dynver).
- A GitHub workflow that packages the plugin for each browser and attaches it to every GitHub release.

## 🏗️ Where is this used?

The full list of projects that rely on this configuration is defined in [graph.json](.github/graph.json).

## 🤔 Should I use this in my projects too?

Only if you want to, but this exists mainly for my own convenience.
I would, however, argue that these settings are reasonable defaults for many browser plugins written in Scala.

More likely, if you're starting a new project, you'll want to use the downstream template [Scala Browser Plugin Template](https://github.com/SgtSwagrid/scala-browser-plugin-template).

## 🔨 How can this be used?

You have several options:

1. If you want continuous updates as this repository evolves, open a PR to add your project(s) to [graph.json](.github/graph.json).
   You'll also need to send me a [PAT](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) with write access to the corresponding repositories.
2. If you want continuous updates, but want to deviate from my template according to your own needs, fork this repository and _then_ add your project(s) to [graph.json](.github/graph.json) (after removing the existing projects from the list). In this case, you can add the PAT yourself.
3. If you just want the settings without the updates, start from [Scala Browser Plugin Template](https://github.com/SgtSwagrid/scala-browser-plugin-template) (for a new project), or simply copy and paste the files (for an existing project).

## 👮‍♂️ License

The included MIT license should be considered only as part of the template, and is not binding.
This repository is hereby released to the public domain, to be used freely.
In particular, and contra [LICENSE.md](LICENSE.md), you may remove the license text from copies.

## 👁️ See also

- [Scala Browser Plugin Template](https://github.com/SgtSwagrid/scala-browser-plugin-template) is a full template which uses this configuration.
- [Omnibrowser](https://github.com/SgtSwagrid/omnibrowser) is the library with which the plugins are written, and the sbt plugin which builds them.
- [Scala Config](https://github.com/SgtSwagrid/scala-config) is an upstream template for Scala 3 projects in general.
