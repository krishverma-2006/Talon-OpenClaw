# Talon OpenClaw

**Control your devices from the command line or Telegram.**

Talon OpenClaw is a TypeScript project powered by [Bun](https://bun.com). It brings device control into two familiar places: a local CLI and Telegram. Use the interface that fits the moment to send commands to your connected devices.

> **Project status:** This README is based on the project description and the supplied Bun commands. Add the specific supported devices, commands, and Telegram setup details as those become available.

## What it does

- **CLI control:** Run the project locally and interact with your devices from a terminal.
- **Telegram control:** Send commands through Telegram, making device control available from a chat.
- **TypeScript and Bun:** The application entry point is `index.ts`, and Bun handles dependency installation and execution.

## Requirements

- [Bun](https://bun.com) (the project was initialized with Bun v1.4.2)
- A Telegram bot and its credentials, if you plan to use Telegram control
- The device connections and configuration required by your setup

## Install

Clone or download this project, open a terminal in its directory, and install dependencies:

```bash
bun install
```

## Run

Start the application with:

```bash
bun run index.ts
```

Follow the prompts or instructions printed by the application to use its CLI or Telegram features.

## Telegram setup

Telegram control requires the bot configuration expected by the application. Create a bot with Telegram's BotFather, then provide its token and any other required settings using the configuration method implemented by this project.

**Do not commit bot tokens or other secrets to source control.** Store credentials in an environment variable or a local configuration file excluded from Git. Check the application code for the exact variable names and setup steps.

## How the project runs

`index.ts` is the command-line entry point used in the run command above. Bun executes the TypeScript source directly and installs the packages declared by the project. The application can then connect its command handling to the CLI and Telegram interfaces and issue operations to the devices configured for it.

## Development

Install dependencies before running the application:

```bash
bun install
bun run index.ts
```

## Contributing

Contributions and ideas are welcome. When opening an issue or pull request, include the device or integration involved, the steps to reproduce any problem, and relevant logs with private credentials removed.

## License

No license has been specified yet. Add a `LICENSE` file before distributing or accepting contributions under particular reuse terms.
