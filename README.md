# How AI Connects Inc. - AI Platform

<p align="center"><code>npm i -g @openai/codex</code><br />or <code>brew install --cask codex</code></p>

<p align="center"><strong>How AI Connects AI Platform</strong> - Enterprise-ready AI-assisted development built on OpenAI Codex technology.
</br>
</br>A comprehensive ecosystem bridging artificial intelligence and practical software development.</p>

## About This Platform

The **How AI Connects Inc. AI Platform** extends OpenAI's Codex with enterprise-grade capabilities, enhanced security, and comprehensive integration options. Built for developers, teams, and organizations who need reliable, secure, and powerful AI-assisted development tools.

**Key Features:**

- 🚀 **Multi-Modal Access**: CLI, IDE integration, Web interface, and SDK/API
- 🔒 **Enterprise Security**: Sandboxed execution, zero data retention options, comprehensive approvals
- 🔌 **Extensible**: Model Context Protocol (MCP) support and custom agent framework
- 🎯 **Developer-First**: Intuitive tools that enhance existing workflows
- 📊 **Production-Ready**: Built with Rust for performance and reliability

### Platform Options

- **CLI**: Interactive terminal interface - `codex` command runs locally on your computer
- **IDE Extensions**: Native integration for VS Code, Cursor, Windsurf - <a href="https://developers.openai.com/codex/ide">install in your IDE</a>
- **Web**: Cloud-based access via <a href="https://chatgpt.com/codex">chatgpt.com/codex</a>
- **SDK**: Programmatic access for automation and custom integrations

> 📖 **Learn More**: See our [Platform Vision](./VISION.md) and [Company Overview](./COMPANY.md) to understand our mission and strategic direction.</p>

<p align="center">
  <img src="./.github/codex-cli-splash.png" alt="Codex CLI splash" width="80%" />
  </p>

---

## Quickstart

### Installing and running Codex CLI

Install globally with your preferred package manager. If you use npm:

```shell
npm install -g @openai/codex
```

Alternatively, if you use Homebrew:

```shell
brew install --cask codex
```

Then simply run `codex` to get started:

```shell
codex
```

If you're running into upgrade issues with Homebrew, see the [FAQ entry on brew upgrade codex](./docs/faq.md#brew-upgrade-codex-isnt-upgrading-me).

<details>
<summary>You can also go to the <a href="https://github.com/openai/codex/releases/latest">latest GitHub Release</a> and download the appropriate binary for your platform.</summary>

Each GitHub Release contains many executables, but in practice, you likely want one of these:

- macOS
  - Apple Silicon/arm64: `codex-aarch64-apple-darwin.tar.gz`
  - x86_64 (older Mac hardware): `codex-x86_64-apple-darwin.tar.gz`
- Linux
  - x86_64: `codex-x86_64-unknown-linux-musl.tar.gz`
  - arm64: `codex-aarch64-unknown-linux-musl.tar.gz`

Each archive contains a single entry with the platform baked into the name (e.g., `codex-x86_64-unknown-linux-musl`), so you likely want to rename it to `codex` after extracting it.

</details>

### Using Codex with your ChatGPT plan

<p align="center">
  <img src="./.github/codex-cli-login.png" alt="Codex CLI login" width="80%" />
  </p>

Run `codex` and select **Sign in with ChatGPT**. We recommend signing into your ChatGPT account to use Codex as part of your Plus, Pro, Team, Edu, or Enterprise plan. [Learn more about what's included in your ChatGPT plan](https://help.openai.com/en/articles/11369540-codex-in-chatgpt).

You can also use Codex with an API key, but this requires [additional setup](./docs/authentication.md#usage-based-billing-alternative-use-an-openai-api-key). If you previously used an API key for usage-based billing, see the [migration steps](./docs/authentication.md#migrating-from-usage-based-billing-api-key). If you're having trouble with login, please comment on [this issue](https://github.com/openai/codex/issues/1243).

### Model Context Protocol (MCP)

Codex can access MCP servers. To configure them, refer to the [config docs](./docs/config.md#mcp_servers).

### Configuration

Codex CLI supports a rich set of configuration options, with preferences stored in `~/.codex/config.toml`. For full configuration options, see [Configuration](./docs/config.md).

---

### Platform Documentation

> 📘 **Documentation Guide**: New to our documentation? Check out the [Documentation Overview](./DOCUMENTATION.md) for a quick reference to all our docs.

#### Vision & Strategy

- [**Platform Vision**](./VISION.md) - Our mission, vision, and strategic direction
- [**Company Overview**](./COMPANY.md) - About How AI Connects Inc.

#### Getting Started

- [**Getting started**](./docs/getting-started.md)
  - [CLI usage](./docs/getting-started.md#cli-usage)
  - [Slash Commands](./docs/slash_commands.md)
  - [Running with a prompt as input](./docs/getting-started.md#running-with-a-prompt-as-input)
  - [Example prompts](./docs/getting-started.md#example-prompts)
  - [Custom prompts](./docs/prompts.md)
  - [Memory with AGENTS.md](./docs/getting-started.md#memory-with-agentsmd)

#### Configuration & Security

- [**Configuration**](./docs/config.md)
  - [Example config](./docs/example-config.md)
- [**Sandbox & approvals**](./docs/sandbox.md)
- [**Authentication**](./docs/authentication.md)
  - [Auth methods](./docs/authentication.md#forcing-a-specific-auth-method-advanced)
  - [Login on a "Headless" machine](./docs/authentication.md#connecting-on-a-headless-machine)
- [**Zero data retention (ZDR)**](./docs/zdr.md)

#### Automation & Integration

- **Automating Codex**
  - [GitHub Action](https://github.com/openai/codex-action)
  - [TypeScript SDK](./sdk/typescript/README.md)
  - [Non-interactive mode (`codex exec`)](./docs/exec.md)
- [**Advanced**](./docs/advanced.md)
  - [Tracing / verbose logging](./docs/advanced.md#tracing--verbose-logging)
  - [Model Context Protocol (MCP)](./docs/advanced.md#model-context-protocol-mcp)

#### Development & Community

- [**Contributing**](./docs/contributing.md)
- [**Install & build**](./docs/install.md)
  - [System Requirements](./docs/install.md#system-requirements)
  - [DotSlash](./docs/install.md#dotslash)
  - [Build from source](./docs/install.md#build-from-source)
- [**FAQ**](./docs/faq.md)
- [**Open source fund**](./docs/open-source-fund.md)

---

## About How AI Connects Inc.

**How AI Connects Inc.** is dedicated to democratizing AI-assisted development and making advanced AI capabilities accessible, reliable, and seamlessly integrated into every developer's workflow. We build enterprise-ready platforms that empower developers and organizations worldwide.

**Our Vision**: To bridge the gap between artificial intelligence and practical software development  
**Our Mission**: To enhance productivity, accelerate innovation, and maintain the highest standards of quality and security

Learn more in our [Platform Vision](./VISION.md) and [Company Overview](./COMPANY.md).

---

## License

This repository is licensed under the [Apache-2.0 License](LICENSE).

Built on OpenAI Codex technology. Copyright 2025 How AI Connects Inc.
