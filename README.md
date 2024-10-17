# jacamo-cli - APT Package for [JaCaMo CLI](https://github.com/jacamo-lang/jacamo-cli)

## DESCRIPTION
This package provides the JaCaMo CLI, a command-line interface tool to create and manage JaCaMo projects for Debian, Ubuntu, and derivates.

The JaCaMo project aims to promote the Multi-Agent Oriented Programming (MAOP) approach by providing a development platform that integrates tools and languages for programming the following dimensions of Multi-Agent Systems: agents (Jason), environment (Cartago), and organisation (Moise).

The JaCaMo platform is distributed under the licences of each platform, i.e. available open source and under GNU LGPL.

## INSTALATION
To install the JaCaMo execute the following commands in a terminal:
```
echo "deb [trusted=yes] http://packages.chon.group/ chonos main" | sudo tee /etc/apt/sources.list.d/chonos.list 
sudo apt update
sudo apt install jacamo-cli
```

## USING
To execute the JaCaMo execute the following commands in a terminal:
```
jacamo app create multiagentSystem --console
cd multiagentSystem
jacamo multiagentSystem.jcm 
        
        Runtime Services (RTS) is running at 127.0.0.1:46687
        Agent mind inspector is running at http://127.0.0.1:3272
        CArtAgO Http Server running on http://127.0.0.1:3273
        Moise Http Server running on http://127.0.0.1:3274
        [Moise] OrgBoard o created.
        [Moise] group created: g1: group1 using artifact ora4mas.nopl.GroupBoard
        [Cartago] Workspace w created.
        [Cartago] artifact c1: example.Counter(3) at w created.
        [bob] join workspace /main/o: done
        [bob] join workspace /main/w: done
        [bob] focusing on artifact c1 (at workspace /main/w) using namespace default
        [bob] focus on c1: done
        [bob] focusing on artifact g1 (at workspace /main/o) using namespace default
        [bob] focus on g1: done
        [bob] focusing on artifact o (at workspace /main/o) using namespace default
        [bob] focus on o: done
        [bob] hello world.
```

## INFO
See the [JaCaMo web site](https://jacamo-lang.github.io/).


## COPYRIGHT
Boissier, Olivier, Rafael H. Bordini, Jomi F. Hübner, Alessandro Ricci, e Andrea Santi. “Multi-Agent Oriented Programming with JaCaMo”. Science of Computer Programming 78, nº 6 (junho de 2013): 747–61. https://doi.org/10.1016/j.scico.2011.10.004.


<details>
<summary> Cite using Bibtex </summary>

```
@article{jacamo,
title = {Multi-agent oriented programming with JaCaMo},
journal = {Science of Computer Programming},
volume = {78},
number = {6},
pages = {747-761},
year = {2013},
note = {Special section: The Programming Languages track at the 26th ACM Symposium on Applied Computing (SAC 2011) & Special section on Agent-oriented Design Methods and Programming Techniques for Distributed Computing in Dynamic and Complex Environments},
issn = {0167-6423},
doi = {https://doi.org/10.1016/j.scico.2011.10.004},
url = {https://www.sciencedirect.com/science/article/pii/S016764231100181X},
author = {Olivier Boissier and Rafael H. Bordini and Jomi F. Hübner and Alessandro Ricci and Andrea Santi},
keywords = {Multi-agent oriented programming, Autonomous agents, Shared environments, Agent organisations}
}
```
</details>