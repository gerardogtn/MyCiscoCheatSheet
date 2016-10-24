# Contributing

We follow a couple of guidelines in order to make this project well structured
and easy to follow. Before contributing, make sure to follow these.

## Guidelines
1. There's a directory per device (currently only switches and routers).
2. In each directory there is a GLOBAL.md document that describes common global
configuration.
3. Each directory is organized by topic. For example, router/DynamicRounting.md
shows the configuration of RIPv2 OSFP, among others.
4. Before listing a command, indicate the configuration mode in which the
command must be executed. For instance, to configure the hostname of a switch
or router you'd write:
``#(config) hostname $NEW_HOST_NAME$``
5. As in the previous example, variables are prefixed and postfixed by a `$`
and the variable is in Upper Case.

## Go and contribute!
That's about it, post any issues that you find and make sure that this project
is as complete as possible.
