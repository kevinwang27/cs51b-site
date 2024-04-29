---
title: 'Project 1:  Convergence'
layout: default
nav_order: 1
parent: Projects
---

# Project 1: Convergence

## Introduction

Welcome to the first project of CS 51B! In this project, you will use what you learned from the Frontend Masters Bootcamp to build a browser-based multiplayer word game called Convergence. We have provided the backend of this app; you will create the frontend.

By the end of this project, you should have a fully functional game that users can play. You will even be able to deploy the app if you choose to make it accessible for everyone online!

A walkthrough of this project spec in video form can be found below.

<iframe width="560" height="315" src="https://www.youtube.com/embed/D36lgepGr9s?si=Nn5vvGJapLy1rAbc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Convergence Rules

The easiest way to understand the rules is to watch the demo portion of the walkthrough above. You can also play around with the staff's solution to this project at [google.com](google.com).

{: .note }
Your frontend can and should be better! Our barebones version simply shows the basic game functionality.

### Basic Rules

The objective of the game is for the players to converge on a single word. The game starts with each player submitting a word. After that, each round proceeds as follows:

1. The unique submitted words from the previous round are the new target words for the current round.
1. If there was only one unique word (all words matched), then the players have converged and the game is finished!
1. Otherwise, based on the target words, each player will come up with a new word that hasn't been used before.
1. The first N words submitted will be taken as the round's submitted words, where N is the number of unique target words.
1. Repeat from step 1.

Valid words must be a single word (no spaces) and new (not used in a previous round).

## Architecture

* Diagram
* Text overview

### Pub/Sub + Ably

* Explain pub/sub and the Ably service
* Link to Ably realtime docs

### Backend server

* Explain backend server API and how it uses Ably channels/presence
* Link to convergence repo README (API spec and message types)

## Assignment

* Implement frontend!

### Setup

* (Recommended) WSL
* Install golang
* Download zip

### Skeleton code

* Backend is done in server.go and others
* Frontend in views/
* Some Ably functionality done and comments with how to use the lib?

### Running Locally

* ABLY_KEY=<key> go run server.go