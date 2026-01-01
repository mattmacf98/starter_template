# Node JS Starter Template

This repository provides starter files to help you run your code against the Buildium test harness.

## What's Included

- **Dockerfile** — A base image that extends the test harness image. Copy your app binary into it and run the harness against your code.
- **app** - a script that gets coppied into your bin to act as a bridge between runnign an executable and invoking the generated `main.js`
- **Makefile** — Handles building your project binary, copying over `meta.json` and `app`, and running the Docker image to test your solution.

## Getting Started

1. Replace the `FROM` directive in the Dockerfile with the base test harness image provided by the tutorial author.
2. Create a `.env` file with your credentials (see `.env.example` for an example).
3. Update `meta.json` with your project ID from the Buildium website. When you're ready, set the `stage` value to the stage you want to test against.
