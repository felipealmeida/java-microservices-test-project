
# Introduction

This is a project definition to test how a junior developer deals with
Java technologies which he may or may not know.

It also tests how the developer uses the git repository.

## Git organization repository

This exercise must be given as a git repository link that the
evaluator can clone.

It is expected that the commit messages are well organized and follow
a pattern. For example, it should not change formats mid-way and each
commit should always do one single thing.

## Documentation

The project should have a minimum documentation on how to set-up, how
to compile, what are its dependencies (which versions if that matters)
and how to run and test it.

## Docker

It is highly desirable that any runtime dependencies can be set-up
with a docker-compose.yml made available by the project itself. That
helps with repeatability and with the learning curve from newer
contributors.

## Project definition

The project consists in creating a Spring-Boot application with Kafka
and ElasticSearch integration. The project should read from Kafka
(there are multiple ways, you should consider which is best, and why),
and save the message in a ElasticSearch server.

The message format should be defined by the application (but must be
JSON) and must be validated by the application.

The message must contain three values: longitude, latitude and a name.

The Java service must be able to read the message, interpret it, print
to console, and save it to a ElasticSearch.
