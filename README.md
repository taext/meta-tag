# Introducing the meta-tag v10.2

### and the meta-data operator 



march 3rd 2018 by d@v1d.dk

a worldboy.org white paper

<img src="meta-tag_logo_4.png" alt="Drawing" width=300/>

<br>

## scope and value proposition

The meta-tag

1. is an open-source general-purpose explicit meta-data format
2. adds a hierarchical dimension to the tag concept

<br>





## definition

1. a meta-tag is a tag with optional tags

2. a meta-tag can grow in two dimensions

    - sibling, denoted `.` 

    - child, denoted `..`

<br>

For the sake of completeness of definition, only the last sibling can have children. 

This follows naturally from the syntax and seems to work nicely in practice.

<br>

## 1. the prefix `..` meta-data operator

### 1.1. the basic meta-tag

Here is an example of the basic meta-tag:

**..podcast**

using the `..` prefix meta-data operator to indicate meta-tag format. 

While this meta-tag contains only the single word `podcast`, the `..` prefix effectively sets the word in the tag domain context, visually and parsing-wise.

### 1.2. implicit object referencing

The *prefix* `..` meta-data operator is an *implicit* reference. That is to say, the object being described is only implicitly connected to the tag. 

E.g. a web page, text paragraph or line of text containing the meta-tag:

    +45 31 27 34 66 ..Michael Manboy..mobile.phone.work..Work Harder Inc..

This example of a phone number with explicit meta-data demonstrates the full syntax at work.

Here are the final two syntax components, used in this example, completing the meta-tag definition:

1.  by convention, title-case tags are considered title/text tags

2. the trailing `..` allows for white-space (normally `_` underscore)

<br>

## 2. the `.` sibling operator

Here is an example of a meta-tag with multiple tags 

**..mp3.podcast.american.tech**

This meta-tag describes an implicit object with the tags
 
 - mp3
 - podcast
 - american
 - tech

 All four tags describing the object itself, as if branching out to form a star.


 More cerebrally, the `.` single dot operator is a separator of several tags *in the same dimension*, all describing the dimension above/below/around the corner.

 But importantly, the `.` single dot operator is just classic tag functionality as known from Evernote tags, Flickr tags etc.

 <br>

 ## 3. the in-line `..` meta-data operator
 
 When the `..` meta-data operator occurs in-line, *it signifies a branch*. 
 
 The following tags, separated by `.` single dots, will describe the tag preceding the `..` meta-data operator.
 
 Thereby forming a new branch of descriptive dimension. 
 
 This is more easily understood visually - here is a more elaborate version of the previous example:

**..mp3..filetype.longform.podcast..american.tech**

or in expanded view


- mp3
  - filetype
  - longform
  - podcast
    - american
    - tech

<br>

Created in real-time simply by asking open questions appropriate to the tag in question

    Q. "what kind of a podcast?" 
    A. "an American podcast", "a tech podcast" 

and 

    Q. "MP3 what?" 
    A. "MP3 filetype", "long-form MP3", "MP3 podcast"

<br>

This kind of *free-form tag type declaration* if you will, is of course only one particular use of the meta-tag. 

Though it is my favourite way  at the moment of wrapping my head around the concept.

I hope you can think of uses, musings and abuses. 

Drop me a mail if you do.