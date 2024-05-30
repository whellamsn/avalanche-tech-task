# Avalanche Tech Task

## Introduction

Welcome to the Avalanche tech task. Thanks for taking the time to attempt this. Please note the following:

1. This is just to give us a rough idea of your skills and approach - there is no 'right' or 'wrong' way to accomplish this task
2. We don't expect a fully featured, fully tested application
3. Anything you don't complete, please mention so we know you had it in mind. Anything you might want to improve, please also mention.
4. You are free to use whatever resources (Google / Stack Overflow) you would if coding normally
5. Treat this like a normal pairing session and don't be afraid to ask for clarification if something is unclear

## Pre-requisites

- docker
- node (v18.17+)

## Getting Started

1. `docker-compose up`

**On the first run you will need to wait for the composer_installation container to finish.** On subsequent runs the vendor modules are there already so it should complete immediately.

This should spin up a PHP JSON game api available on http://localhost:8080

Hit the endpoint for brief instructions on how to use the API.

## Objectives

Set up a NEXT application. The easiest way to do this is with:

`npx create-next-app@latest`

It will prompt you with some set up questions. You can use Typescript if you want.

Within the application:

- Add a basic homepage, with a nice welcome message
- Link to game list page, populated via the API
- Add a basic game information page (details below)

The game list page needs the game image and the game name.

Each game on the list page needs a link to a more detailed game info page, again populated via the game API.

The game info page needs to diplay the following information:

- Name
- Description
- Category
- Return to player (RTP) (this is a percentage)
- Bonus round
- Price from & to (this value is in pence)
- Instructions
- T&Cs
- Game image

In addition, if the game is a jackpot game, it needs some kind of banner on the image indicating this.

There needs to be a way to launch the game(S) from the list and info page. The game launcher will be added later, but you should hit /game/launcher/{game-slug}

Ideally your pages will use a clean, appropriate layout and presentation.

This will include a suitable header and footer with mininal stylng, but think about responsive design as most of our customers use a device to access the site.

This is not a design task, but being able to make something functional and easy to navigate is appreciated.

## Things to Consider

- Tests
- Caching/loading
- Error handling
- Game search
- Presentation
- Ease of use
- Documentation
