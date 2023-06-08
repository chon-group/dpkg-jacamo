# jacamo-cli - Debian Package for [JaCaMo CLI](https://github.com/jacamo-lang/jacamo)

## DESCRIPTION
This package provides the JaCaMo CLI, a command-line interface tool to create and manage JaCaMo projects, for Debian and derivates.

The JaCaMo project aims to promote the Multi-Agent Oriented Programming (MAOP) approach by providing a development platform that integrates tools and languages for programming the following dimensions of Multi-Agent Systems: agents (Jason), environment (Cartago), and organisation (Moise).

The JaCaMo platform is distributed under the licences of each platform, i.e. available open source and under GNU LGPL.

## INSTALATION
```console
echo "deb [trusted=yes] http://packages.chon.group/ chonos main" | sudo tee /etc/apt/sources.list.d/chonos.list 
sudo apt update
sudo apt install jacamo-cli
```

## USING
```console
jacamo app create multiagentSystem --console
cd multiagentSystem
jacamo multiagentSystem.jcm 
        > Task :compileJava
        > Task :processResources NO-SOURCE
        > Task :classes

        > Task :buildJCMDeps
        reading from file multiagentSystem.jcm ...
        file multiagentSystem.jcm parsed successfully!

        JCM packages dependencies updated at .jcm-deps.gradle

        BUILD SUCCESSFUL in 1s
        2 actionable tasks: 2 executed
        > Task :compileJava UP-TO-DATE
        > Task :processResources NO-SOURCE
        > Task :classes UP-TO-DATE

        > Task :run
        Runtime Services (RTS) is running at 192.168.1.9:46687
        Agent mind inspector is running at http://192.168.1.9:3272
        CArtAgO Http Server running on http://192.168.1.9:3273
        Moise Http Server running on http://192.168.1.9:3274
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

## COPYRIGHT
See the [JaCaMo web site](https://jacamo.sourceforge.net/).
