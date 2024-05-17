+++
title = "Brenno Lemos"
path = "resume"
template = "resume.html"

[extra]
sub = "Master of Computer Science, Software Engineer & Linux Nerd 🐧"
profile_picture = "../img/me.jpg"
+++

# EXPERIENCE

{{ job_entry(
    title="Rust development on a Loyalty Program's system",
    role="Senior Backend Developer",
    at="Arionkoder / iSeatz",
    time_windows=["APR 2024 — PRESENT"])
}}

<p class="justify">
At Arionkoder, I was outstaffed to iSeatz, a software company in the loyalty program business. I was invited to continue the development of a new Rust microservice, using the Axum framework, as well as SQLx for compile-time checked queries and Insta for unit testing.
</p>

{{ job_entry(
    title="Fullstack development on a Web System for clinic management",
    role="Senior Backend Developer",
    at="ZarpSystem / iClinic",
    time_windows=["JUL 2021 — APR 2024"])
}}

<p class="justify">
At ZarpSystem, I was outstaffed to iClinic, a clinic management software company. I was responsible for developing new features to an existing software, which included Fullstack work with Python & Django (REST API) for the Backend and JavaScript/TypeScript & React for the Frontend.
</p>

<p class="justify">
The development team was guided with the agile approach Scrum, with ceremonies like Dailies and two-week Sprints.
</p>

<p class="justify">
The job also involved requirements gathering with the Product Owner, development of unit tests and CI/CDs. Local development was handled via Docker Containers.
</p>

<p class="justify">
Our team was challenged with decoupling some of the most critical components of the Monolithic system into new Microservices. That included handling user login across different products and replicating and synchronizing required data to ensure the product’s resilience.
</p>

# EDUCATION

{{ education_entry(
    title="Master of Computer Science",
    role="Federal University",
    at="São João Del-Rei",
    started="FEB 2022",
    ended="MAR 2024",
    score="93.60%")
}}

After graduating in Computer Science, I was invited by a couple of professors to pursue a Master's degree. During this journey, I have:

- Been granted a scholarship by [FAPEMIG];
- Given a lecture about the Rust Language and its security features ([SECOMP 2022]). [Documents][rust-secomp-2022] and [Video][rust-secomp-2022-video];
- Enrolled into a professor's internship program, which saw me teaching classes and developing a C library for game development ([jogo.h]). More about the latter below;
- Given a 4 hour corse on the Rust Language for a class of 30 students ([SECOMP 2023]), teaching from the basics all the way to advanced features such as monomorphism and polymorphism. [Slides in Portuguese][rust-secomp-2023];
- Developed an open source software for developing, simulating, plotting and modifying Ordinary Differential Equations (ODEs), written fully in Rust, as part of my thesis ([Software][ode-designer-rs] & [Article][master-thesis]);

[FAPEMIG]: https://fapemig.br/
[SECOMP 2022]: https://secomp2022.wixsite.com/secomp2022
[rust-secomp-2022]: https://github.com/Syndelis/rust-secomp-2022
[rust-secomp-2022-video]: https://www.youtube.com/watch?v=bIZ_0OIbhg8&feature=youtu.be&ab_channel=BrennoLemos
[jogo.h]: https://github.com/syndelis/jogo.h
[SECOMP 2023]: https://secomp.ufsj.edu.br/programacao-secomp/minicursos#todos_minicursos
[rust-secomp-2023]: https://secomp2023.brenno.codes/
[ode-designer-rs]: https://github.com/Syndelis/ode-designer-rs
[master-thesis]: https://github.com/Syndelis/dissertacao-mestrado

{{ education_entry(
    title="Bachelor of Computer Science",
    role="Federal University",
    at="São João Del-Rei",
    started="FEB 2018",
    ended="DEC 2021",
    score="93.35%")
}}

During my time at the University, I have:
- Been granted several scolarships for student tutoring and research & development;
- Participated in study groups about Computer vision and Computational Modelling;
- Participated in lectures ([SECOMP 2019]) about Data Science, Game Development, Web Development;
- Studied Artificial Intelligence, Machine Learning, Bio-Inspired Algorithms, Ranking and Sorting Methods, Optimization, Operational Systems, Computer Architecture, Robotics, Math & Statistics, [and many other courses];
- Enrolled into an internship which later led to a job at ZarpSystem;

[SECOMP 2019]: https://secomp.ufsj.edu.br/home
[and many other courses]: https://ccomp.ufsj.edu.br/images/documentos/Fluxograma_CC-UFSJ.pdf

# PROJECTS

{{ job_entry(
    title="Development of scientific softwares for the construction and simulation of mathematical and computational models",
    role="Federal University",
    at="São João Del-Rei",
    time_windows=["JUL 2018 — MAR 2021", "FEB 2022 — DEC 2023"])
}}

During my graduation, I collaborated with a professor in the development of a software that allows researches to construct mathematical and computational models via an intuiditve GUI, simulate in-place, export the results and even generate equivalent Python code.

The [software for Cellular Automatas] is a Qt desktop application made with C, Pyhton and Cython. The project was funded by [FAPEMIG].

During my pursuit of a Master's degree, we've once again partnered to develop a [similar software][ode-designer-rs] that allows researchers to create and simulate ODEs, written entirely in Rust. The software ships with an ImGui-based interface featuring a node editor. It's capable of generating Python code to simulate equations, is localized in English and Portuguese and is extensible via Python code. Saving and loading data has been handled with Serde.

[software for Cellular Automatas]: https://github.com/Syndelis/ac-designer

{{ job_entry(
    title="Development of a library to facilitate game creation in C, jogo.h",
    role="Federal University",
    at="São João Del-Rei",
    time_windows=["SEP 2022 — DEC 2022"])
}}

During my professor's internship (as part of my Master's), I have been tasked with creating the freshmen students' last assignment. The assingment I came up with involved the development of a game in C, in order to have the students exercise what they learned about control flow statements and data structures.

As C is no easy language and neither are the libraries for developing graphical applications wihth it, I took to myself the task of developing a library that facilitates the creation of games. The library is capable of drawing primitives, rendering static and animated sprites, rendering text, playing sounds and making all complex matrix transformations that OpenGL allows.

Most of those operations usually require pre-loading assets as to not waste the computer's resources, but since the library's main design goal was to be as simple as possible to use and learn, I've applied caching and memoization techniques to minimize boiler-plate code required when using [the library][jogo.h].

The library is also [fully documented] using Doxygen and GitHub Actions for automatically deploying updated versions.

[fully documented]: https://syndelis.github.io/jogo.h

{{ job_entry(
    title="Development of a low-level game engine with a Python interface, the Eel Engine",
    role="Personal Project",
    at="",
    time_windows=["MAR 2020 — SEP 2022"])
}}

The project aims to provide a more user-friendly, pythonic and powerful alternative to the popular but outdated PyGame library. As such, the [Eel Engine] is a modern-interfaced game engine for Python.

The engine is written in C, for performace, and interfaced to Python via the usaged of Cython.

[Eel Engine]: https://github.com/syndelis/eel-engine

{{ job_entry(
    title="Development of a 3D souls-like game in Godot",
    role="Personal Project",
    at="",
    time_windows=["JUL 2021"])
}}

As a challenge to myself, I decided to try and make a complete 3D game in the short span of two weeks. [The result][isosouls] is an isometric *souls-like* RPG complete with traps, bosses and loot!

[isosouls]: https://github.com/Syndelis/IsoSouls

# FREELANCING & OTHERS

{{ job_entry(
    title="Development of a leaderboard system to connect users from Steam to Discord",
    role="Freelancer",
    at="Oxonian Games",
    time_windows=["2021 - 2022"])
}}

I was tasked with developing a leaderboard system that can connect users from Steam to Discord.

Therefore, I developed a C++ dynamic library (.SO + .DLL) for the GameMaker Studio 2 game to utilize and communicate with an API server made in Express.js, using a MariaDB database to keep the user’s scores. There’s also a Python Discord bot that fetches the data in order to interact with users.

{{ job_entry(
    title="Library & Tools development, Linux porting",
    role="Freelancer",
    at="Soulchild Game",
    time_windows=["2019 - 2021"])
}}

[Soulchild] is an upcoming Metroidvania platformer coming to Windows, MacOS and Linux on Steam developed in GameMaker Studio 2. I’ve contributed towards development by making several libraries and also by porting it to Linux.

[Soulchild]: https://store.steampowered.com/app/1609020/Soulchild/

{{ job_entry(
    title="Student tutoring on General Programming, Data Structures, Sorting Algorithms and more",
    role="Federal University",
    at="São João Del-Rei",
    time_windows=["JUL 2018 - DEC 2021"])
}}

Ever since my first academic year until the very last I’ve had scholarships for student tutoring. They’ve arguably made me a better teacher, as well as a better learner
