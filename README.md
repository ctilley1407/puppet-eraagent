# eraagent

#### Table of Contents

1. [Description](#description)
2. [Setup - The basics of getting started with eraagent](#setup)
    * [Beginning with eraagent](#beginning-with-eraagent)
3. [Usage - Configuration options and additional functionality](#usage)
4. [Limitations - OS compatibility, etc.](#limitations)
5. [Development - Guide for contributing to the module](#development)

## Description

eraagent is the daemon deployed to clients/nodes connecting back to a central Eset Management Server (ESMC).

This module installs the package(s) require for the Eset Remote Management Agent and enables and starts the daemon/service.

## Setup

### Beginning with eraagent

`include eraagent` should be enough to get the daemon installed.

### Recommended base parameters

`
class { 'eraagent':
      eraa_server_hostname      => $eraa_server_hostname,
      eraa_http_proxy_hostname  => $eraa_http_proxy_hostname,
      eraa_http_proxy_port      => $eraa_http_proxy_port
}
`

## Limitations

This module has been tested on CentOS 7 and OEL 7-8.

This module was developed to install the eraagent service to enable deployment of the eraagent service across linux at a large scale

## Development

Development on this module is welcome to better support RHEL base OS. Currently, there is no clean way to deploy the Eraagent across linux distributions.

## Contributors

To see who's already involved, see the [list of contributors.](https://github.com/ctilley1407/puppet-eraagent/graphs/contributors)
