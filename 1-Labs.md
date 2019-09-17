# Functions Labs

In each of the following labs you'll explore a different aspect of Oracle
Functions from creating, to deploying, to troubleshooting, to invoking.  In all
cases you'll be using the `fn` CLI extensively so you may find these references
helpful:

* [fn Commands
  Cheatsheet](https://github.com/sachin-pikle/functionslab/wiki/Functions-Commands-Cheatsheet)

* [fn CLI docs](https://github.com/fnproject/docs/blob/master/cli/README.md)

## Java Functions

Fn provides an FDK (Function Development Kit) for each of the core supported
programming languages.  But the Java FDK is the most advanced with support for
Maven builds, automatic function argument type conversions, and comprehenive
support for function testing with JUnit.

The [Introduction to Java Functions](4-Java-Functions.md) lab covers all these
topics and more.

## Troubleshooting

If you've been following the instructions in the tutorials carefully you
shouldn't have run into any unexpected failures--hopefully!!  But in real life
when you're writing code things go wrong--builds fail, exceptions are thrown,
etc.  Fortunately the
[Troubleshooting](5-Troubleshooting.md) tutorial
introduces techniques you can use to track down the source of a failure.

## Automatically invoke Functions using OCI Events service

OCI Events service lets you monitor OCI resource changes and send notifications
and/or trigger a function automatically in response to that change. We'll
explore sending email notifications, and invoking a function via the OCI Events
when an image is uploaded to an OCI Object Storage bucket in [Automatically
invoke Functions using OCI Events](9-Functions-Invoke-OCI-Events.md).

## Containers as Functions

One of the coolest features of Fn is that while it's easy to write functions in
various programming languages, you can also deploy Docker images as functions.
This opens up entire worlds of opportunity as you can package existing code,
utilities, or use a programming language not yet supported by Fn.  Try the
[Containers as Functions](6-Container-as-Function.md)
tutorial to see how easy it is.