# ansible-role-cloudprepare
An Ansible role to prepare cloud hosts to mitigate provider specific pecularities

Most cloud providers use predefined usernames where they deploy your ssh keys. Some have even more local configuration that requires more and more guesswork. If you need to work with different providers, public and private, it can be quite cumbersome to build your code so that it works with all these different defaults.

This role is more or less a brute force approach to find out which defaults work on which of your hosts. The hosts are then put into groups so you can define per group rules for connecting.

TBD: An optional set of tasks creates a common user you can then connect to independently of local defaults.
