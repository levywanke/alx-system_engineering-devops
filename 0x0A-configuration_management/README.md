onfiguration Management with Puppet

## Introduction
This project focuses on Configuration Management using Puppet. Puppet is a widely used open-source configuration management tool that automates the provisioning, configuration, and management of servers. The tasks in this project involve creating Puppet manifests to achieve various configuration management objectives.

## Installation
To run the Puppet manifests in this project, ensure that you have Puppet installed on your Ubuntu 20.04 LTS system. You can follow these steps to install Puppet:

1. Install Ruby and required dependencies:
    ```
    $ apt-get install -y ruby=1:2.7+1 --allow-downgrades
    $ apt-get install -y ruby-augeas
    $ apt-get install -y ruby-shadow
    $ apt-get install -y puppet
    ```

2. Install puppet-lint:
    ```
    $ gem install puppet-lint
    ```

## Usage
### Manifests
1. **0-create_a_file.pp**: Creates a file in `/tmp` with specific permissions, owner, group, and content.
    ```
    puppet apply 0-create_a_file.pp
    ```

2. **1-install_a_package.pp**: Installs Flask package from pip3 with version 2.1.0.
    ```
    puppet apply 1-install_a_package.pp
    ```

3. **2-execute_a_command.pp**: Executes a command to kill a process named `killmenow` using `pkill`.
    ```
    puppet apply 2-execute_a_command.pp
    ```

### Example
```
puppet apply 0-create_a_file.pp
puppet apply 1-install_a_package.pp
puppet apply 2-execute_a_command.pp
```

## Project Structure
```
0x0A-configuration_management/
│
├── 0-create_a_file.pp
├── 1-install_a_package.pp
├── 2-execute_a_command.pp
├── README.md
└── ...
```

## Credits
This project is a part of the ALX Software Engineering program, provided by ALX Africa in collaboration with Holberton School.

Copyright © 2024 ALX, All rights reserved.
