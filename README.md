# CAPED SHELL

This is a simple 80LOC restricted shell to put in /etc/passwd.

## Help

capedsh

    Usage: capedsh -F FILE -IGNORED -c COMMAND
    
    Open a caped/restricted shell that only allows the commands listed
    in "/etc/capedsh".
    
    This file accepts the following format:
    =COMMAND       : Will allow executing "COMMAND ARGUMENTS...".
    @COMMAND       : Will allow executing "COMMAND".
    !ssh-copy-id-n : Allow "ssh-copy-id".
    !ssh-copy-id-1 : Allow "ssh-copy-id", but only one key.
    @passwd        : Allow changing the password with "passwd".
    
    You can create a restricted user with "useradd -m -s /bin/capedsh USER".

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
