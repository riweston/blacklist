# UBNT EdgeMax dnsmasq DNS blacklisting and redirection

[![License](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/britannic/blacklist/blob/master/LICENSE.txt) [![Alpha  Version](https://img.shields.io/badge/version-v0.06--alpha-red.svg)](https://github.com/britannic/blacklist) [![GoDoc](https://godoc.org/github.com/britannic/blacklist?status.svg)](https://godoc.org/github.com/britannic/blacklist) [![Build Status](https://travis-ci.org/britannic/blacklist.svg?branch=master)](https://travis-ci.org/britannic/blacklist) [![Coverage Status](https://coveralls.io/repos/github/britannic/blacklist/badge.svg?branch=master)](https://coveralls.io/github/britannic/blacklist?branch=master) [![Go Report Card](https://goreportcard.com/badge/gojp/goreportcard)](https://goreportcard.com/report/github.com/britannic/blacklist)

[community.ubnt.com](https://community.ubnt.com/t5/EdgeMAX/Self-Installer-to-configure-Ad-Server-and-Blacklist-Blocking/td-p/1337892)

NOTE: THIS IS NOT OFFICIAL UBIQUITI SOFTWARE AND THEREFORE NOT SUPPORTED OR ENDORSED BY Ubiquiti Networks®

## Copyright

* Copyright © 2018 Helm Rock Consulting

## Overview

EdgeMax dnsmasq DNS blacklisting and redirection is inspired by the users at [EdgeMAX Community](https://community.ubnt.com/t5/EdgeMAX/bd-p/EdgeMAX)

## Licenses

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1; Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
1; Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

The views and conclusions contained in the software and documentation are those
of the authors and should not be interpreted as representing official policies,
either expressed or implied, of the FreeBSD Project.

## Features

* Generates configuration files used directly by dnsmasq to redirect dns lookups
* Integrated with the EdgeMax OS CLI
* Any FQDN in the blacklist will force dnsmasq to return the configured dns redirect IP address

## Compatibility

* update-dnsmasq has been tested on the EdgeRouter ERLite-3, ERPoe-5, ER-X, UniFi Security Gateway USG3 routers, EdgeOS versions v1.7.0-v1.9.7+hotfix.4
* integration could be adapted to work on VyOS and Vyatta derived ports, since  EdgeOS is a fork and port of Vyatta 6.3

## Installation

### EdgeRouter ERLite-3, ERPoe-5 & UniFi-Gateway-3

* sudo dpkg -i edgeos-dnsmasq-blacklist_0.0.7_mips.deb

### EdgeRouter ER-X & ER-X-SFP

* sudo dpkg -i edgeos-dnsmasq-blacklist_0.0.7_mipsel.deb

## Removal

### EdgeMAX ERLite-x & EdgeMax ER-X

* sudo apt-get remove edgeos-dnsmasq-blacklist

> blacklist





- - -
Generated by [godoc2md](http://godoc.org/github.com/davecheney/godoc2md)
