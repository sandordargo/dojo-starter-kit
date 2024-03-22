# Coding dojo starter kit

In this repository, you'll find links to a couple of resources you can use for hosting coding dojos as well as some pieces of advice. Though some parts are language-agnostic, in general, I'm focusing on C++.

## General recommendations
- The goal of a coding dojo is to practice and learn. Therefore, don't try to solve production issues because inevitable you'll start focusing on delivering something by the end of the session instead deeply understand the problems you're facing.
- Try to set aside 90-120 minutes each week for a dojo. Longer sessions would be too tiring and it would be also unrealistic to find so much time, and shorters are not enough to immerse yourselves in the problem.
- Set up an environment before you start the session.
- If you run an in-person dojo where multiple environments have to be set up, share at least a day in advance the kata you'll use for the practice.
- For online dojos, try to follow a mob-like setup, with the below roles. Don't forget to regularly switch roles!
  - The driver is at the keyboard. The driver is not "thinking", just typing.
  - The navigator tells the driver what to write.
  - The rest is called the mob. They observe and call out if they see some problems with the code being written.
- At the end of a session, don't forget to review what you learned at a session. For some, it will be language features, for others architectural patterns or maybe even how to teach effectively.
- It's OK to keep doing the same exercises over and over again. Just as you'd do at a sports training.
- It's OK to fail.

## How to find exercises

Here are a few sources:
- [CodingDojo.org](https://codingdojo.org/kata/)
- [CodeKata.com](http://codekata.com/)
- [A coding dojo exercises plan towards refactoring legacy code](https://philippe.bourgau.net/a-coding-dojo-exercises-plan-towards-refactoring-legacy-code/)
- [Racking Kar Katas](https://github.com/emilybache/Racing-Car-Katas)
- [The Gilded Rose Refactoring Kata](https://github.com/emilybache/GildedRose-Refactoring-Kata)
- [Emily Bache's GH in general...](https://github.com/emilybache)
  
## Environment

Starting a new project in certain languages is as easy as a breeze. C++ is not among those languages, though important advancements have been made during the last few years.

In order not to waste half of the dojo setting up a new repository, it's important that you start hosting the dojo with a project that is ready to be built.

You can use [cmake-project-creator](https://github.com/sandordargo/cmake-project-creator) to generate a new project. Run it with `python3 create_cmake_project.py -n <ProjectName> -d examples/single.json -o <output parent dir>`, and you will get a new project set up in `<output parent dir>/<project_name>` with a `cmake` project with two libraries, one for production code and one for tests. Once generated, you can build and run the tests with `./runTests.sh`. It requires that you have a C++ compiler, `cmake` and `conan` or `conan2` installed. For more info, check out [cmake-project-creator's README](https://github.com/sandordargo/cmake-project-creator).
