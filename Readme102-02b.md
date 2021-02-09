# introduction

_lets talking about git but let's first explain Version Control._

## Version Control

>> it is a system that allows you to revisit various versions of a file or set of files by recording changes, and can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes.

# Centralized Version Control

The need for collaboration within a developer team on a single file or set of files led to the advent of the Centralized Version Control System, and this system entails a single server storing all changes and file versions, which can be accessed by various clients. This streamlined the collaboration process

## Let's talk a little bit about Distributed Version Control :
```
A Distributed Version Control systems (DVCS) addresses the major vulnerability of the CVS: the server as a single point of failure.
If a CVS goes down, collaborators cannot work with each other on a file or save changes and new versions.
Also, in the event of corruption of a central database’s hard disk — with the absence of backups — all work will be lost,
except for any portions on local machines.
```
__\*To prevent this type of catastrophic loss, a DVCS allows clients to create mirrored repositories. 
These data backups can be easily be placed on the server to replace any lost information.__ 

# So, what is Git?
Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project Git creates a snapshot of the file and stores a reference to it.
