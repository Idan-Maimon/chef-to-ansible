# bnhp-linux Cookbook

This cookbook is part of the B&H Photo Linux baseline configuration and is used to install and configure various components on the system. The following sections provide an overview of the cookbook's purpose and functionality.

## Purpose

The purpose of this cookbook is to provide a baseline configuration for B&H Photo Linux systems. It installs and configures various components such as SELinux, firewalld, and xauth, and sets up the `/root/.bash_profile` file.

## Features

- Installs and configures SELinux
- Installs and configures firewalld
- Installs and configures xauth
- Sets up the `/root/.bash_profile` file

## Usage

To use this cookbook, simply include it in your Chef run. The cookbook has the following attributes:

- `bnhp-linux['network_manager']`: Specifies whether the network manager should be enabled or disabled. Defaults to `false`.
- `bnhp-linux['policy']`: Specifies the SELinux policy. Defaults to `'disabled'`.
- `bnhp-linux['target-policy']`: Specifies the SELinux target policy. Defaults to `'targeted'`.
- `bnhp-linux['firewalld-policy']`: Specifies the firewalld policy. Defaults to `'disabled'`.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please submit a pull request or open an issue on the GitHub repository.

## License

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see <http://www.gnu.org/licenses/>.

## Files

- `rhel_baseline_collection/roles/rh_security/tasks/bash_profile.yml`: Sets up the `/root/.bash_profile` file.