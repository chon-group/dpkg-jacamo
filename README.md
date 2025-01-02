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
+ The [JaCaMo project](https://github.com/jacamo-lang/jacamo) aims to promote the Multi-Agent Oriented Programming (MAOP) approach by providing a development platform that integrates tools and languages for programming the following dimensions of Multi-Agent Systems: agents, environment, and organisation.

---
+ ___JaCaMo-CLI Debian Package___ is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/). The licensor cannot revoke these freedoms as long as you follow the license terms:

    * __Attribution__ — You must give __appropriate credit__ like below:

    Lazarin, N.M., Pantoja, C.E., Viterbo, J. (2024). Dealing with the Unpredictability of Physical Resources in Real-World Multi-agent Systems. In: Rocha, A.P., Steels, L., van den Herik, J. (eds) Agents and Artificial Intelligence. ICAART 2023. Lecture Notes in Computer Science(), vol 14546. Springer, Cham. [https://doi.org/10.1007/978-3-031-55326-4_3](https://www.researchgate.net/publication/378961821_Dealing_with_the_Unpredictability_of_Physical_Resources_in_Real-World_Multi-agent_Systems)

    <details>
    <summary> Cite using Bibtex </summary>

        @InProceedings{lazarin_2024,
        doi="10.1007/978-3-031-55326-4_3"
        author="Lazarin, Nilson Mori
        and Pantoja, Carlos Eduardo
        and Viterbo, Jos{\'e}",
        editor="Rocha, Ana Paula
        and Steels, Luc
        and van den Herik, Jaap",
        title="Dealing with the Unpredictability of Physical Resources in Real-World Multi-agent Systems",
        booktitle="Agents and Artificial Intelligence",
        year="2024",
        publisher="Springer Nature Switzerland",
        address="Cham",
        pages="48--71",
        isbn="978-3-031-55326-4"
        }
    </details>