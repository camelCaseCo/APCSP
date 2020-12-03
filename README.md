# APCSP <a name="top"></a>
Repository for all things regarding my APCSP class.

---

This repository contains the source code as well as, in some cases, a selection of precompiled binaries pertaining to projects I have completed in my APCSP class.

For licensing information, please consult [LICENSE.md](/LICENSE.md).

---

# Projects
## [Unit 4](/Unit-4/README.md) <a name="unit4"></a>
The Unit 4 project is a simple game with a text-based UI in which the user attempts to pick up trash on the road. Go to the project page to learn more.

---

# What are Binaries? What is Source Code? <a name="types-of-downloads"></a>
Programmers create programs using programming languages. Some popular programming languages include JavaScript, Python, C#, Java, and many more. On its own, a program is nothing more than text in a file. The term source code refers to this plaintext code. But if code is just normal text, where does the magic happen? Depending on the programming language being used, the magic can happen in one of two places:

- Interpreter
- Compiler

An interpreter is the simpler of these two explain. An interpreter is a special type of application which can read the program and run it. Interpreters can run programs immediately, but they are almost never as fast as compilers. So what is a compiler? A compiler is similar to an interpreter, but instead of running the program immediately, it instead translates the program into binary code which the computer can run directly. The fact that the computer can now run the code directly is why compiled code can basically always run faster than interpreted code, which must be run through software. However, unlike an interpreter, a compiler has to take time to translate the program into binary code before the program can be run. Therefore, a compiler cannot run the code immediately.

Because interpreters can run code immediately, interpreters and interpreted languages are used in situations when it is more important to run code immediately than it is to run it as fast as possible. A good example of this is a website. The code that makes up a website is usually some combination of HTML, CSS, and JavaScript. These are all interpreted languages, and your browser - probably Google Chrome, Mozilla Firefox, or Microsoft Edge - acts as the interpreter for the code. The fact that they are interpreted languages allows you to see and interact with the website immediately.

However, compilers are favored in situations when it is more important to run code efficiently than it is to run it immediately. For example, compiled languages are used when programming videogames. It's not important to be able to run the code immediately after writing it, but if you have lots of fancy graphics and other mechanics, then it is important to have code which is as efficient as possible.

There is another advantage to compiled languages over interpreted languages, and that is that with a compiled language, only the programmer needs to have the compiler software. This is because once the programmer writes their code, they can use the compiler to translate it into binary code, and then let users download the binary code. But with an interpreter, the _users_ need to have the interpreter software, because it will be interpreted on their machines. In fact, you already have experience with this dynamic - think about it. If you want to look at a website, you _have_ to use a browser. This is because the browser interprets the code that makes up the website on the spot. But if you want to play a videogame that you downloaded, you don't need a special application to run it, you just _run_ it. This is because you downloaded binary code which has already been translated from the source code using a compiler.

There is a catch though - if two computers have different CPUs (the brains of the computer), such as a 32-bit CPU, a 64-bit CPU, or an ARM CPU, or if the computers are running on different Operating Systems - like Windows, Linux, or macOS, then the binary code for each computer will look different. This means that if you want to write compiled code which can run on lots of different machines, you will have to compile it once for each different machine that you want it to be able to run on. This is why if you are downloading an application on the internet, you will see different options for Windows, Linux, and macOS.

### So What Does This Mean for Me?
When you want to download an application found in this repository, you will be presented with the option to either download a pre-compiled binary, or to compile the binary from source. Basically, you can either download binary code which has already been compiled for you, or you can download the actual source code and then compile it yourself. If you don't know a lot about programming and there is a pre-compiled binary which has been compiled specifically for your machine, then it is probably best to just use the pre-compiled binary. However, there are a _lot_ of different machines, and I couldn't possibly compile a different version for every type of machine in the world. So, there are some machines that I haven't made a pre-compiled binary for. If you are on one of these machines - an ARM machine, or a macOS machine - then you will likely need to download the source code and compile the program yourself. Not to worry though! I've made a step-by-step guide for compiling every application in this repository, so you don't need to worry about a thing.

---

# Why the Warning? <a name="why-the-warning"></a>
If you downloaded a pre-compiled binary of one of the applications on this website, and you are ona Windows machine, then chances are you got a message from your computer the first time you ran the program telling you that the application might be dangerous. Why is this?

To begin with, let me make something clear - none of the applications of downloads in this repository are intentionally malicious or dangerous in any way. (The reason I say intentionally is because I cannot guarantee that it's impossible for someone to hack this repository, but it's pretty damn unlikely).

So, if there isn't any malicious code to be found, then why is the message popping up?

To understand that, we first have to understand how Windows determines whether or not it can trust a certain application. When Windows runs an applicatino for the first time, it will look for a cartificate - basically a fancy secure digital signature - which is attached to the file. The certificate will contain information about who wrote the software, who published it, who owns the copyright, etc. If Windows finds such a certificate, it will use that information to determine whether or not the application can be trusted.

The reason that Windows gets fussy about the applications in this repository is because it doesn't find a certificate, and the reason that it doesn't find one is because there isn't one to be found. At this point, I have neither the time nor the experience to invest in getting a certificate issued for myself, and in any case, there wouldnt be a _whole_ lot of merit - these are small-scale school projects, not enterprise-scale software applications.

In summary, the reason Windows gets fussy about my applications is because I haven't gotten a certificate issued with which to sign said applications, and the reason I haven't gotten a certificate issued is because at this point in time and for this application, I believe that it simply isn't worth the effort. If you still feel uncomfortable with the message, consider the following options:
- Run a virus scan on the application before running it to ensure that there is no malicious code.
- Download the source code and compile it yourself instead of using a pre-compiled binary. This allows you to be certain that there is no malicious code, because you can actually look at the program itself before you compile it, as opposed to just trusting that there isn't anything sneaky hidden within the unintelligible ones and zeroes of a binary executable.

---

# .NET, Dependent, and Standalone <a name="dotnet-dependency"></a>
What is .NET? What is a .NET-Dependent Binary? What is a Standalone Binary?

To start, let's define a binary. Put simply, a binary is a program which is written in ones and zeroes. Most programmers don't write the ones and zeroes by hand, instead they use a programming language which is made of more human-readable text, and then use special software to translate that code into binary. Read the section on [binaries and source code](#types-of-downloads) to learn more about this.

Now that we know what a binary is, what is .NET? .NET is a **software framework** developed by Microsoft. It is open-source, which means that the source code is publicly avaliable and anyone can contribute to it, and it will run on Windows, Linux, or macOS. .NET provides a lot of useful tools that applications can use, which means that those applications don't need to include those tools within their own code. Think of .NET as a helper for applications. .NET also provides tools and programming languages that you can use to create applications, but that isn't relevant right now.

In essence, the difference between a .NET-dependent application and a standalone application is that a .NET-dependent application relies on .NET for some of the tools that it needs in order to function properly, while a standalone application brings all the tools that it needs along with it. On the one hand, stanalone applications are sometimes better because they don't need a framework like .NET to be installed on a machine in order to run properly. On the other hand, framework-dependent applications are usually much much smaller, both in terms of download size and in temrs of how much space they take up on your computer, due to the simple fact that they don't need to bring all of their tools with them - their tools are already waiting for them at the jobsite.

In the end, it's really up to you which one to go with. I have presented you with the information as it stands, and it is now up to you to make your decision on whether to download .NET alongside a .NET-dependent binary, or to just download a standalone binary on its own.

---

# Contact Information
For questions regarding any application or guide contiained within this repository, please email [dev@nekoboi.com](mailto:dev@nekoboi.com) with the subject line `github:apcsp:questions-concerns`.

For any other communication regarding this repository, please email [dev@nekoboi.com](mailto:dev@nekoboi.com) with the subject line `github:apcsp:misc`.

For anything else, please email [dev@nekoboi.com](mailto:dev@nekoboi.com) with the subject line `gen:<desc>`, where `<desc>` is a short but descriptive description of the topic of your email.

---

# Other Platforms
#### YouTube: [dev nekoboi](https://www.youtube.com/channel/UCQ4SDqGYFNa8e7wSSgKc69g/featured)
#### Discord: nekoboi#0001

---

### [Back to Top](#top)
