# Welcome

This is a github org, documentation and set of repos (currently just one) by and for the VB community!

## OSS from the VB Community

The following list are projects that are not only of interest/benefit to most VB developers, but are also primarily built in VB.  So if you are interested in getting more involved in open-source as a VB dev... check these out!

### [CSharpToVB (powered by 'Roslyn')](https://github.com/paul1956/CSharpToVB)

Paul has been working on a pretty incredible and completely free C# to VB conversion tool that is powered by the Roslyn API.  It is (as of this writing) seeing continued improvements on a very regular basis.  If you have a need to convert C# to VB... check this thing out!

### [Code Coverage](https://github.com/paul1956/Code-Coverage)

Using Visual Studio 2019 Community alongside unit testing?  Be sure to check out Paul's excellent utility to assist you in reviewing how well your tests are actually testing your code.

### [x8086NetEmu](https://github.com/morphx666/x8086NetEmu)

This is so cool that it has to be included it here!  Xavier has created a working 8086 emulator.  There are a few things that aren't 100% working; but, for the most part, it's working pretty much as well as other offerings in this space... and it's written in VB!

### [Community.VisualBasic (alternative to the Microsoft.VisualBasic library)](https://github.com/DualBrain/Community.VisualBasic)

Want to have all of the ease-of-use features that VB provides regardless of the project type and/or target operating system?  Enter [Community.VisualBasic](https://github.com/DualBrain/Community.VisualBasic), the *.netstandard 2.0* community driven alternative to the official Microsoft.VisualBasic "runtime".  

[Community.VisualBasic](https://github.com/DualBrain/Community.VisualBasic) Goals:

- Compatibility with Microsoft.VisualBasic namespace/functionality.  
- Cross-platform capability/compatibility.
- Slice and dice into smaller packages.
- Publish as separate nuget packages.
- Add additional functionality where appropriate.

See [Community.VisualBasic](https://github.com/DualBrain/Community.VisualBasic) for more details.

### [Vazor](https://github.com/VBAndCs/Vazor)

A VB Razor framework for ASP.NET Core 6 (MVC and Razor Pages).

### [VB to WebAssembly Compiler (Proof-of-Concept)](https://github.com/biocad-cloud/data.ts/releases/tag/v0.5.136-alpha)

Although not a much more than a proof-of-concept at this stage, it is a great start on creating an independent WebAssembly compiler for VB.

> NOTE: since the commit [9466098](https://github.com/biocad-cloud/data.ts/tree/9466098937eb30f80f77d3b17b6f37878d047170), wasm compiler module for VB.NET language was move to a new individual project, and the new compiler project called [``VanillaBasic``](https://github.com/dotvanilla/vanilla).

### Category: VisualBasic.NET Machine Learning & Data Science Library

#### 1. [LibOptimization](https://github.com/tomitomi3/LibOptimization)

LibOptimization is a numerical optimization library that simplifies optimization using C#, VisualBasic.Net and other .NET Framework languages. This library is used by people who need optimization such as science (eg physics), engineering, sound, finance, statistics, medical care, structural design etc.

#### 2. [sciBASIC](https://github.com/xieguigang/sciBASIC)

A framework for developing the general data science application in VB.NET language. The sciBASIC framework provides a set of library module api for:

1. math algorithm
2. data mining and machine learning
3. data visualization
4. I/O for data with multiple general common used file formats in data science area
5. general application framework for develop console pipeline application.

#### 3. [Darwinism](https://github.com/xieguigang/Darwinism)

``Darwinism`` project is a high performance parallel computing toolkit for VisualBasic.NET data science application running on unix mono/.net 5.

## **VB Welcome Here** (OSS that is VB friendly...)

The following projects ("pocket communities") that, although aren't built in or specificaly for VB, are generally positive toward the VB developer.

Note that some will have documentation/samples specifically for VB while others simply ensure that their projects work regardless of what development language utilizes them. 

- [FluentFTP](https://github.com/robinrodricks/FluentFTP): An FTP and FTPS client for .NET & .NET Standard, optimized for speed. Provides extensive FTP commands, File uploads/downloads, SSL/TLS connections, Automatic directory listing parsing, File hashing/checksums, File permissions/CHMOD, FTP proxies, FXP support, UTF-8 support, Async/await support, Powershell support and more.
- [NAudio](https://github.com/naudio/NAudio): Audio and MIDI library for .NET.
- [DynamicAudioNormalizer](https://github.com/lordmulder/DynamicAudioNormalizer): Dynamic Audio Normalizer is a library for advanced audio normalization purposes. It applies a certain amount of gain to the input audio in order to bring its peak magnitude to a target level (e.g. 0 dBFS). However, in contrast to more "simple" normalization algorithms, the Dynamic Audio Normalizer dynamically re-adjusts the gain factor to the input audio. This allows for applying extra gain to the "quiet" sections of the audio while avoiding distortions or clipping the "loud" sections. In other words: The Dynamic Audio Normalizer will "even out" the volume of quiet and loud sections, in the sense that the volume of each section is brought to the same target level. Note, however, that the Dynamic Audio Normalizer achieves this goal without applying "dynamic range compressing". It will retain 100% of the dynamic range within each "local" region of the audio file.

## Resources

### [Code samples for VB.NET](https://github.com/karenpayneoregon/visual-basic-getting-started)

Karen has been working on moving her samples (collected over the years on, I believe, TechNet) to a repo here on github.  There's some really good stuff in here!

### [GotBASIC.com - VB7+](https://gotbasic.com/vb.html)

Cory has a website dedicated to BASIC with a section for VB v7+ with a lot of great resources.

---

## Discussion

Discussion pertaining to VB.NET takes place in the form of issues in this repo, under the Discussion section.

If you want to suggest a feature, discuss current design notes or proposals, etc., please begin the discussion in the Discussion section.

It is beneficial to have language ideas discussed nearby to where the design artifacts are. Comment threads that are short and stay on topic are much more likely to be read. If you leave comment number fifty, chances are that only a few people will read it. To make discussions easier to navigate and benefit from, please observe a few rules of thumb:

- Discussion should be relevant to Visual Basic .NET language and related technologies. Issues that are not will be summarily closed.
- Choose a descriptive title for the issue, that clearly communicates the scope of discussion.
- Stick to the topic of the issue title. If a comment is tangential, start a new issue and link back.
- If a comment goes into detail on a subtopic, also consider starting a new issue and linking back.
- Is your comment useful for others to read, or can it be adequately expressed with an emoji reaction to an existing comment?

## VB.NET Language Implementation

The reference implementation of the Visual Basic .NET language can be found in the [Roslyn repository](https://github.com/dotnet/roslyn). Until recently, that was also where language design artifacts were tracked. Please allow a little time as we move over active proposals.

