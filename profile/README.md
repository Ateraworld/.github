# Atera

[Website](https://ateraworld.github.io/#/)

-----

[Download Android](https://play.google.com/store/apps/details?id=com.ateraworld.atera)

[Download IOS](https://apps.apple.com/it/app/atera-ferrate-trekking/id6449359062)

-----

<p align="center">
  <img src="https://github.com/Ateraworld/.github/assets/31132987/6982dafb-1acc-41af-abfc-3ed4446a318d" width=1280>
</p>


# Contributing

We allow people who love the project and the idea to contribute in creating the **activities reports and relations**.

To begin a collaboration, send an email to `atera.world@gmail.com` and we will contact you back as soon as possible 😁.

## Setup environment

To start contributing, we will provide you the following tools:

- `atera CLI`: a command line tool to facilitate some tasks such as report validation and creation
- `atera_vscode`: an extension for [vscode](https://code.visualstudio.com/), that perfectly integrates **Atera** with the development environment. It enables to dinamically reference activities, photos and points of interests inside your reports.

To propose changes, create a pull request in the [atera_data](https://github.com/Ateraworld/atera_data) repository, we will check the proposed reports and push them on our backend after all checks have passed.

## Steps

### atera_data

Clone the [atera_data](https://github.com/Ateraworld/atera_data) repository:
```sh
git clone https://github.com/Ateraworld/atera_data.git
```

### atera CLI   

The `atera CLI` is a single self contained _.exe_ file. 
It is recommended to add the directory in which the file is placed to the `path` system env variable to be able to call the CLI from everywhere, to do this follow the [tutorial](https://www.wikihow.com/Change-the-PATH-Environment-Variable-on-Windows).
To initialize the _.conf_ folder, run:
```sh
atera help
```
After its first run, the CLI will create the config folder in the same directory of the executable. Inside the folder there will be a configuration file called _local.json_.

Edit the file and set the `root` entry to the absolute path of the cloned **atera_data** repository, in this way the CLI will be able to access the existing data.

### atera_vscode  

Install the _.vsix_ extension in vscode:
```sh
code --install-extension <path_to_the_atera_vsix>
```

Go into vscode settings and search for _atera_. 
All the settings will be displayed, set the entry `dataRoot` to the absolute path of the cloned **atera_data** repository.

## You are done!
Happy development and thank you for helping us in creating the best database of outdoor activities!
