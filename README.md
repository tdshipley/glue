![Pipeline Logo](https://upload.wikimedia.org/wikipedia/commons/3/37/The_Great_Wave_of_Kanagava.jpg)

# Pipeline

Pipeline is a framework for running a series of tools.  Generally, it is intended as a backbone 
for automating a security analysis pipeline of tools.

# Installation

gem install pipeline

# Extending Pipeline

Pipeline is intended to be extended through added "tasks".  To add a new tool, 
copy an existing task and tweak to make it work for the tool in question.

# Usage

pipeline <image>

# Basic Options

For a full list of options, use `pipeline --help` or see the OPTIONS.md file.

# Dependencies

* clamav
* hashdeep
* rm (*nix)
* git
* mount (*nix)
* docker

# Development

To run the code, run the following from the root directory: 
>ruby bin/pipeline <options> target

To build a gem, just run: 
gem build pipeline.gemspec

# Configuration files

For advanced usage scenarios, you can save your configuration and use it at runtime.


# License

Apache 2:  http://www.apache.org/licenses/LICENSE-2.0