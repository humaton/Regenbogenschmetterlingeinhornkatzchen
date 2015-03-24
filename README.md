# Regenbogenschmetterlingeinhornkätzchen

This is pre alpha software, its aim is to ease development with containers on exotic platforms like Windows or Mac.

CDK expects you to have installed vagrant, if not you can do so here https://www.vagrantup.com/downloads
And downloaded boxes with following names:  rhel-7.0, rhel-7.1-atomic, centos-server-7, centos-atomic-7
(box downloading will be part of this project soon)

##Installation

There are two ways how to install cdk

###From source
```bash
git clone git@github.com:humaton/regenbogenschmetterlingeinhornkatzchen.git
cd regenbogenschmetterlingeinhornkatzchen
gem build regenbogenschmetterlingeinhornkatzchen.gemspec
gem install regenbogenschmetterlingeinhornkatzchen-0.0.2.gem
```

###Rubygems
```bash
$gem install regenbogenschmetterlingeinhornkatzchen
```
##Usage
regenbogenschmetterlingeinhornkatzchen uses vagrant so you can use usual vagrant commands once inside project directory.

Install CDK vagrant plugins:
```bash
$regenbogenschmetterlingeinhornkatzchen vagrant --install-cdk-plugins
```

Create new project with centos-atomic backend for container deployement:
```bash
$regenbogenschmetterlingeinhornkatzchen new --name gabelspahler --host centos-atomic
$cd gabelspahler
$regenbogenschmetterlingeinhornkatzchen run
```
More info:
```bash
$regenbogenschmetterlingeinhornkatzchen --help
```

