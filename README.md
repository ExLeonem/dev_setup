
# Automation of local development setup
A personal base setup for my development machines. To automatically perform the setup follow the guid at [How to run the setup](#How-to-run-the-setup).

Check [asdf](https://github.com/asdf-vm/asdf-plugins) for more tools and languages.



## Requirements:
- Ansible (tested with 2.9.6)
- Linux (tested with ubuntu 20.04 & 19.10)
- English directory naming & base directories like (~/Downloads, ~/Desktop, ~) with write/read permission


<!-- ``
sudo ansible-pull https://github.com/ExLeonem/ansible_dev_machine
`` -->


## How to run the setup


1. Pull the repository and install the required roles

``
    ansible-galaxy install -r requirements.yml
``
<br/>
<br/>

2. Execute the playbook to install all tools and applications

``
ansible-playbook -K main.yml
``


## Applications & Tools to be installed


| To be installed | Category 
| ---             | ---    
| zsh             | shell
| [oh-my-zsh](https://ohmyz.sh/)       | theme
| [docker](https://www.docker.com/)          | virtualisation, development
| [elixir](https://elixir-lang.org/) v.1.10.3 | Programming language
| [erlang](https://www.erlang.org/) v.22.3.3 | Programming language
| [nodejs](https://nodejs.org/en/) v.14.0.0 | Programming language
| [rust]() v.1.43.1, nightly | Programming language
| [FiraCode](https://github.com/tonsky/FiraCode)        | Font
| [VS-Code ](https://code.visualstudio.com/)        | Editor
| [Gulp Tasks](https://marketplace.visualstudio.com/items?itemName=nickdodd79.gulptasks)       | VS-Code Extension
| [ES7 React Snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)      | VS-Code Extension
| [vscode-elixir](https://marketplace.visualstudio.com/items?itemName=mjmcloug.vscode-elixir)      | VS-Code Extension
| [Shades of Purple](https://marketplace.visualstudio.com/items?itemName=ahmadawais.shades-of-purple)           | VS-Code Theme
| [tensorman](https://github.com/pop-os/tensorman) | TF package manager
| [meta](https://github.com/mateodelnorte/meta) | Meta-Repository management
| [Sass](https://sass-lang.com/) | CSS transpiler
| [postman](https://www.postman.com/) | REST API testing
| [Slack](https://slack.com/intl/de-de/)| Communication tool
| [anaconda](https://www.anaconda.com/) | Programming language, package manager


## Roadmap
Utilities/Tools/Applications that will be added.

| To be installed | Category 
| ---             | ---    
| [Django]() | library
| [PyTorch](https://pytorch.org/) | library


- [ ] Hardware checks for specific packages (cuda)
- [ ] Parameterize versions