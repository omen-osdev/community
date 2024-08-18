# OMEN project: Week 1 Report. 18 August 2024 - By Tretorn

Hello there!

First of all, thank you all for your interest in this project.
I feel personally grateful for all of your support and the passion
that I see each time I read your messages. We are starting to make
a community. 

We will create weekly reports so you can follow on the current status
of the development. So, without further ado:

## TLDR:

1. Look for your name in the teams section, if you are not present or need to change anything, contact me.
2. Talk to your team mod (if defined) and your peers in the team, discuss the direction you want to take and next steps.
3. Schedule a meeting to start working.
4. Read the Team coordination part of this doc, it is really important.

## License

One thing we need to collectively decide is the **license** we will 
open a poll this week. The only requirement is that the entire project
has to be free and open source.

## Teams

We have the teams, they are as follows:

| Team name                  | Mod email (pending) | Members            | Available hours (GMT+0) | Email (pending) |
|----------------------------|---------------------|--------------------|-------------------------|-----------------|
| Website and documentation  |                     | kaustubhg          |                         |                 |
|                            |                     | ERICBIDOPA.        |                         |                 |
|                            |                     | literallyAmbiguous |                         |                 |
| Maths and Performance      |                     | Iroms              |                         |                 |
|                            |                     | .crisco            |                         |                 |
| Devices and drivers        |                     | spidy09272         |                         |                 |
|                            |                     | toadkarter         |                         |                 |
| Memory                     | jpichel@omendev.org | shubhamraj2002     | 7-9PM                   |                 |
|                            |                     | yash_b             |                         |                 |
|                            |                     | sahilkhan6655      |                         |                 |
|                            |                     | _koliver73         |                         |                 |
| Hardware abstraction layer |                     | theandrewcosta     | 1-3AM                   |                 |
|                            |                     | CarlosM            |                         |                 |
|                            |                     | spleenatsteam      |                         |                 |
|                            |                     | dr.strangelove8885 |                         |                 |
| Utilities and automation   |                     | s1nisteR           | 1-3PM                   |                 |
|                            |                     | noobie_coder       |                         |                 |
| Bootloaders and CPU        | t34@omendev.org     | miike2844          | 10-12PM                 |                 |
|                            |                     | abcdef2909         |                         |                 |
|                            |                     | froste197          |                         |                 |
|                            |                     | tomaragua          |                         |                 |
| Processes                  |                     | korinlu            | 1-3PM                   |                 |
|                            |                     | RisingSkies        |                         |                 |
| Executables                |                     | randomKiwi         |                         |                 |
| Testing and QA             |                     | khraosgenetor      |                         |                 |
|                            |                     | p4nicwave          |                         |                 |
| Platform and environment   |                     | R9_                |                         |                 |
|                            |                     | popher             |                         |                 |
|                            |                     | ST                 |                         |                 |
| Filesystems                |                     | huzx6128           |                         |                 |
| Community managers         |                     | spidy09272         |                         |                 |
|                            |                     | s1nisteR           |                         |                 |

### A few points:

- You can request, at any time, for whatever reason to change teams.
- There is no hierarchy whatsoever inside a team, each member has the same responsabilities as his/her peers.
- Availability hours are merely orientative.
- Come on, hop onto the Filesystems team, don't leave _huzx6128_ alone!
- We will give each one of you email addresses in a few days, please do not misuse them!

### What does each team do?

- Website and documentation:

They will create the website and documentation portal

Contact them when: You create a new feature, they will ask
you to fill some info and to produce some docs.

- Maths and Performance: 

They will implement the most computationally intense algorithms
as well as making sure your code doesn't leaks 3TB of ram per second.

Contact them when: You are ready to release a feature, they will ask
you to run a few tests and perhaps to make some changes.

- Devices and drivers:

They will decide what goes into our supported device list, what does a
driver have to do and test that it actually works.

Contact them when: You want to support a device or you have created a
device driver.

- Memory:

They will implement the physical memory manager, virtual memory manager and
allocators.

Contact them when: You have any doubt about how to get memory to yourself or
how to manage memory maps.

- Hardware abstraction layer:

They will code the specifics of the x86 architecture (and after that some other
architectures).

Contact them when: You need to support any feature from a processor standpoint.
Theese are the assembly guys :D

- Utilities and automation:

They will create scripts and utilities for the project, if you need to have anything
automated ask them for help.

Contact them when: You need an script or program.


- Bootloaders and CPU:

They will code support all the features a modern cpu can handle and make the bootloader
work.

Contact them when: Everything catches on fire, it's probably their fault.

Processes:

This is really a spinoff of the cpu team, they will create the cpu context and process structure
to enable multiple programs to run at the same time.

Contact them when: You need to access a processes data like memory map, pid, etc.

- Executables:

They will create support for ELF executables.

Contact them when: You need to load a process from disk.

- Testing and QA:

They will request for changes and tests in your code, (you have to abide)

Contact them when: You are ready to release a feature or change.

- Platform and environment:

They will manage the servers (when we buy them), and the boot environment (currently gnumakefile)

Contact them when: You need to emulate a new device like a serial device or a nic adapter, also if
the kernel doesn't boot in your machine.

- Filesystems:
  
They will code the different fs drivers: ramfs, ext2, fat32, etc. And the Virtual File System.

Contact them when: You need to read or write a file.

- Community managers:

They will make sure the discord news keep rolling out and giving exposure to the project so you
can use it to hopefully land a cooler job some day.

Contact them when: You want to post a new or something interesting.

### Team coordination

You are autonomous, you can propose new features and make your own decissions. For that and to avoid collisions
with other teams you will have to follow a few rules:

1. Do not affect other modules nor alter folder strucuture.
2. Any changes into the environment have to be consulted with the environment team.
3. All your changes should be marked WIP (Work in progress) until the externally faced interfaces are finished.
4. You should not use a WIP interface from any other team.
5. Once the WIP tag is removed, the interfaces can only be expanded, never modified (if you mess up here, please contac me)
6. Talk with the testing and performance teams before releasing a feature (Releasing = removing the WIP mark)
7. Use correct gitflow (request an issue, create a branch from develop, create pull requests, etc)

## Rules of the server

Can't state this enough, the number one, two and three of the server is: _be kind to others_. Usually whenever
I join an osdev forum or discord server I see a lot of people making fun, condescendant or right out disrespecting
others (usually newbies). This is a safe place to learn, in which you should make whatever is in your hand to help
others in their learning path. We are all in the same boat after all. 

Other things I think are the basics of any server: Don't spam, don't scam, do not distribute illegal material, use
the appropiate forums for posting. That's it :D

## What is each forum for:

### General category:

1. Rules, read only, basic rules of the server.
2. Roles, reaction only, use this channel to get you the roles to see and talk.
3. News, read only, **very important** you need to actively read this channel to be a part of the project.
4. Introduce-yourself, here you can say hi to others and see who joined the server.
5. Meta: To talk about the server itself.
6. Mod-support: If you need anything from the mod team, mention us here and we will dm you. Please do not post the issue directly there.

### Osdev category: 

This category is to talk about osdev in general, things not related to omen, you can talk about other projects aswell.

1. General: To debate about osdev specifics, share news and have heated arguments.
2. show-your-projects: To flex your osdever skills.
3. doubts-learning: To ask questions.
4. no-x86: To ask questions about architectures that are different to x86.
5. offtopic: Please no furry content.

### Omen category:

This category is specifically to talk about the project, not to discus about general osdev.

1. General: To debate about how omen is progressing, architectural decissions, issues, etc.
2. Milestones: To show your contributions and the general progress.
3. Docs: Link to the different documents and references you compile through your journey.
4. Troubleshoot: If you have or see any issue with omen, please post it here!

Other than that, you will have different team chats and voice channels.

