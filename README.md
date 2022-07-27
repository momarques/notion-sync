# notion-sync
A simple tool written in Go to create [Notion](https://www.notion.so) Pages from different sources.

## Why?

I am a musician! An artist!! And I'm also trying to be more organized. 
This project is a CLI tool which automates Notion Page creation based on some specific source of data.

I've started to use Notion a couple months ago and realized it's a powerful tool to organize everything in my life. 
One of the use cases for Notion is to keep track of my music projects.

As I said before, I'm trying to become an artist and for now, I'm only playing and learning with some DAWs and trying to take something out of there. Sometimes I do have some cool stuff, but I just keep forgetting about those projects and don't touch it anymore. 

I've created a couple of Notion templates and one of them is for music projects. This template needs some data to be fulfilled and that's why I need a tool to help me do it, because I'm lazy.

## How?

This tool catches data from available sources and create Notion Pages using those data. It makes use of Notion API to import data, and the source can be anything (plugins).


## Datasources

What kind of sources are available?

I actually thought only about one, which is a simple folder. 
This is the actual implementation that I need for my music projects, which is: read a folder from my computer and create pages for each of the folders. 

I already have like Google Drive sync, etc. on this folder, but I also need a way to document my projects, that's why I'm using Notion for. 

The result expected is: everytime a new folder X is created under a folder Y, it creates a Notion page using a predefined template. All of those specifications are passed through the CLI.

There is also an option `--watch` which watches for a specific datasource and creates the pages without any manual input.

### Different datasources

As I need only this specific datasource, I'm not going to build any other (only when I need). 

That's why I'm building this tool to accept other datasources, but they need to be developed as external plugins and added on the tool.




