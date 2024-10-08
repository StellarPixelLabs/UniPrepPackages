# UniPrepPackages

The target of this file is to help you define and understand what a package here means.   
Each package is defining a set of notes and questions, where later the user can use them to prepare for a test and study.   
Its OK if there are multiple packages for each subject, the user can choose to use a specific package or mix them, obviously there will be overlaps.

## How to use
Simply copy the link for the directory in the repository.   
So you can make multiple packages where each package is a directory in the repository!

## Kind of types
 - Package
 - Close Question
 - Open Question
 - Note

## General define
each type sould be a file so you will have: `pack.json`,`closeq.json`,`note.json`, `openq.json`.   
later I will add tool to test the syntax.   
Every file but `pack.json` should be an array where every element will be as defined bellow.

## How to define

### Pack (MetaData)
file: `pack.json`.   
 - packageUUID:string, use `https://www.uuidgenerator.net/version7`.
 - packageName:string, this is the name will be represented in the package manager.
 - version:string, package version like "1.0.0",it will help keep track.
 - author:string, your alias.
 - course:string, the package course.

### Close Question
file: `closeq.json`.   
 - title:string, the title of the question.
 - desc:string, the question description.
 - tag:string or null, tag will help filter your question, for example, C if its a C lang question.
 - options:string[], array of the answers.
 - answer:number, this is the **index** of the correct answer so from 0 include to 7 include.

### Notes
file: `note.json`.
 - title:string, the title of the note.
 - desc:string, the note desctiption.
 - tag:string or null, tag will help filter your note, for example, C if its a C lang note.
 - course:string, the course that your note is related to.

### Open Questions
file: `openq.json`
 - title:string, the title of the question.
 - desc:string, the question description.
 - tag:string or null, string or null, tag will help filter your note, for example, C if its a C lang question.
 - answer:string, the answer for the question.