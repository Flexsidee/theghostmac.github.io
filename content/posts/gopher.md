+++
title = "Introducing Gopher: How and Why"
date = "2023-07-11"
author = "MacBobby Chibuzor"
description = "Gopher is my Go package manager inspired by Cargo, written in Vim, and driven by the Microkernel architecture."

[taxonomies]
tags = ["showcase", "projects", "Go", "Rust", "architecture"]
+++

---

# Introduction

I am thrilled to announce the launch of [Gopher](https://github.com/theghostmac/gopher), a command-line tool written in Go 
that aims to streamline the management of Go projects. Gopher is designed to 
provide a comprehensive set of features, empowering developers like me to efficiently 
build, test, and run Go applications from the terminal. 
As an avid Rust developer, I drew inspiration from the beloved `cargo` package manager 
and sought to bring its convenience and elegance to the Go ecosystem.

![Gopher Banner](/imgs/gopher-release.png)

## Embracing the Love for Cargo

One of the main motivations behind Gopher is my deep appreciation for the 
Rust language and its accompanying tooling. As I worked extensively with 
Rust's `cargo` tool, I realized how it significantly enhanced my productivity and 
streamlined my workflow.

> Mitchel Hashimoto once said it's easier to continue building a side project when
> you can easily see something good happening from the command line, or at least, from tests.

With `cargo`, you can run the `cargo run` command and see an output, then continue building 
the project until you see the desired output.

Thus, I embarked on the journey to bring a similar experience to the world of Go. 
With Gopher, I hope to provide Go developers with a tool that simplifies project 
management, dependency handling, and testing – just like Cargo does for Rust.

## Exploring the Microkernel Architecture

In the pursuit of building Gopher, I delved into the realm of systems programming and
explored the Microkernel architecture. While it would have been convenient to develop
this tool in Rust, given its well-suited tooling ecosystem, my curiosity led me to choose
Go for this venture. Gopher embraces the principles of the Microkernel architecture,
aiming to maintain a modular and extensible codebase.

This architectural style allows for seamless integration of additional features and
extensions as Gopher evolves over time.

I do not use frameworks when building software, so I did not use Cobra or any CLI framework for Go.

### Features
For now, Gopher supports only the `new` command. You can also append two flags to it:
1. `--web`: to initialize a web application in Go. An entrypoint `cmd/<projectName>` is created for the web app.
2. `--app`: to initialize a normal application in Go.

    ![Gopher Screenshot](/imgs/gopher-demo.png)

If my terminal commands like `z` and `exa` look strange to you, read this [post](https://theghostmac.github.io/posts/rust-tools/).

## A Vim Journey and the Terminal

Another driving force behind Gopher's creation was my desire to master Vim as 
my primary development environment. Prompted by conversations with the 
talented [Timothy Brymes](https://github.com/Brymes), who emphasized the need for
Vim mastery in the Certified Kubernetes Administrator exam, I challenged myself to build 
Gopher using Vim and the terminal alone. By embracing Vim's efficient text editing 
capabilities and working solely from the command line, I aimed to deepen my 
understanding of both Go and Vim while fostering a minimalist development approach.

![Battling with Vim](/imgs/battling-vim.png)

This is me writing Go code in bare Vim 😪.

## Paving the Way for Innovation

Gopher was also born out of a desire to push the boundaries of Go itself. 
Although Go has made significant advancements with features like Generics and the Go 
workspace concept, I wanted to contribute something new to the Go toolchain. 
With Gopher, I aspire to introduce a modern and extensible tool that can adapt to 
evolving developer needs. By building upon the solid foundation of Go, Gopher aims to 
facilitate efficient project management, empower collaborative development, and 
enhance the overall Go development experience.

Gopher is an evolving project, and I am excited to share this initial release with the Go community. 
As I continue to develop and refine Gopher, I welcome feedback, contributions, and ideas from 
fellow developers. Together, we can shape Gopher into a powerful Go tool that empowers 
developers and fosters efficient, enjoyable Go project management.

To learn more about Gopher, explore the repository on [GitHub](https://github.com/theghostmac/gopher). S
tay tuned for updates, additional features, and future releases. 
Let's embark on this journey together as we embrace the simplicity and power of Go development 
with Gopher.

Happy coding! 😄