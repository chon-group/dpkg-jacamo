# jacamo-cli - Debian Package for [JaCaMo CLI](https://github.com/jacamo-lang/jacamo)

## DESCRIPTION
This package provides the JaCaMo CLI, a command-line interface tool to create and manage JaCaMo projects, for Debian and derivates.

The JaCaMo project aims to promote the Multi-Agent Oriented Programming (MAOP) approach by providing a development platform that integrates tools and languages for programming the following dimensions of Multi-Agent Systems: agents (Jason), environment (Cartago), and organisation (Moise).

The JaCaMo platform is distributed under the licences of each platform, i.e. available open source and under GNU LGPL.

## INSTALATION
```console
user@pc:~$ echo "deb [trusted=yes] http://packages.chon.group/ chonos main" | sudo tee /etc/apt/sources.list.d/chonos.list 
user@pc:~$ sudo apt update
user@pc:~$ sudo apt install jacamo-cli
```

## USING
```console
user@pc:~$ jacamo app create multiagentSystem --console

user@pc:~$ cd multiagentSystem/
user@pc:multiagentSystem $ jacamo multiagentSystem.jcm 
[bob] hello world.
[alice] hello world.
```

## COPYRIGHT
See the [JaCaMo web site](https://jacamo.sourceforge.net/).
