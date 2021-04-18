![ph](ph.png "ph")

`ph` is a command-line interface inspired by [heroku](https://devcenter.heroku.com/articles/heroku-cli), [cargo](https://doc.rust-lang.org/cargo/index.html), and [go](https://golang.org/cmd/go/) which aim to make localhost development a bit easier. While some developers will prefer to manage their own environment, I wanted to provide *one* tool to manage PostHog.

`ph` is also a teaching tool.

1. Some developers may not have intimate knowledge of specific tech used by PostHog, `ph` is also a resource for learning those technologies. 
2. With many all-in-one tools if you encounter an error you're left guessing what when wrong. `ph` aims to explain it's actions so that you may sort out your specific environment issues. 

## Prerequisites

- `yarn`
- `git`
- `nodejs` >= 12
- `docker` >= 3.3.0 (to support new Apple chips)

## Supported operating systems

- macOS (and M1 chips)
- Ubuntu
- Windows (via WSL 2)

## Install ph

```sh
% git clone https://github.com/PostHog/ph.git
% cd ph
% yarn install
% yarn link         # puts ph on your path to run from everywhere
```

## Basic commands

```sh
% ph install        # clones and installs dependencies on your machine
% ph up             # starts posthog with docker on your machine
% ph down           # stops posthog
% ph test           # runs posthog test cases
% ph help           # list all cli commands
% ph help [command] # show usage for a specific command
```

## Project status: Experimental

`ph` is experimental and in active development. It's not recommended for use. You can track progress on the [project](PROJECT.md) page. The plan is to make it available once most of the basic commands are finished and tested and the proof of concept verified. There is still a question as to whether this project is worth the effort.