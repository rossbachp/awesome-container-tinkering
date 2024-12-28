# Development Tools - (alpha)

Here you can find information about development tools.

## Editor

### NeoVIM

### VSCode

* YAML SCHEMA

### Jetbrains

### Eclipse

## CI

### Github Actions

### Dagger

### Gitlab

### Gitea

### Jenkins

### Tekton 

## Config Management

### Ansible

### Terraform

### Makefile

### DevBox

[Devbox](https://www.jetify.com/devbox) - "is a tool for creating isolated, reproducible development environments that can run on any system. Unlike Docker or Nix, Devbox simplifies the process by eliminating the need for complex configuration and language-specific dependencies."

Devbox allows developers to set up environments that are consistent, portable, and easy to use, ensuring compatibility across different machines and minimizing setup issues.

### Task

[Task](https://taskfile.dev) - "is a simple, easy-to-use task runner and build tool designed to streamline automation and reduce complexity compared to traditional tools like GNU Make."

Taskfile provides a straightforward approach to managing tasks and workflows, with an emphasis on simplicity and ease of configuration. Task is suitable for developers who want an intuitive and efficient way to automate repetitive tasks without the overhead of more complicated tools.

### Apache Maven

[Apache Maven](https://maven.apache.org) - "is a powerful build automation tool primarily used for Java projects."

Maven simplifies the process of building, managing, and documenting software by providing a centralized way to manage project dependencies, build configurations, and plugin execution. Maven uses XML-based project configuration files (pom.xml) to define project structure, dependencies, and build processes. It also provides repositories for storing and sharing libraries and other resources. Maven is widely used for its ease of integration, standardized build practices, and ability to manage complex multi-module projects.

### Gradle

[Gradle](https://gradle.org) - "is an open-source build automation tool designed for building, testing, and deploying software, with a focus on performance and flexibility."

Gradle supports multiple programming languages, including Java, Kotlin, Groovy, and others. Gradle uses a Domain-Specific Language (DSL) based on Groovy or Kotlin to define builds, and it integrates with other tools like Maven and Ant. Known for its high performance and ability to handle complex builds, Gradle provides incremental builds and parallel execution to improve speed. It’s commonly used in large-scale projects, including Android development, and supports both small and enterprise-level builds.

## GitOps

[GitOps](https://opengitops.dev) is a modern approach to managing Kubernetes clusters and application delivery by leveraging Git as the single source of truth for declarative infrastructure and application definitions. It uses tools to continuously reconcile the desired state stored in Git with the actual state of the cluster, ensuring consistency and enabling automated, version-controlled updates. This method enhances reliability, traceability, and collaboration in DevOps workflows.

Click here for a more curated list for awesome <a href="https://github.com/weaveworks/awesome-gitops">GitOps resources</a>.

### ArgoCD

<a href="https://argo-cd.readthedocs.io/en/stable/">Argo CD</a> - "is a Kubernetes-native GitOps continuous delivery tool that automates the deployment and lifecycle management of applications."

ArgoCD ensures application definitions, configurations, and environments are declarative and stored in version control, providing traceability and auditability. By continuously reconciling the desired state in Git with the actual state in the cluster, Argo CD makes deployments automated, reliable, and easy to manage.

### Flux

<a href="https://github.com/fluxcd/flux2"></a> - "is a Kubernetes-native GitOps tool that ensures clusters stay in sync with configuration sources such as Git repositories or OCI artifacts."

Flux automates deployment updates by applying changes as new code becomes available. Designed for continuous delivery, Flux simplifies managing and versioning infrastructure and application configurations in a declarative manner.

### JenkinsX

## SCM

### GIT

### SVN

## Package Management

### Homebrew

<a href="https://brew.sh">Homebrew</a> - "is a popular, open-source package manager for macOS and Linux, simplifying the installation of software and tools via the command line."

Dubbed "The Missing Package Manager," it streamlines the management of libraries, applications, and dependencies, making it easier for developers and users to set up and maintain their systems.

[Bottles](https://docs.brew.sh/Bottles) in Homebrew refer to precompiled binary packages that make software installation faster and easier. Instead of compiling software from source code, Homebrew can install these prebuilt packages (bottles) directly, saving time and system resources. Bottles are available for most commonly used formulae and are automatically preferred over source installations, making Homebrew efficient and user-friendly. These binaries are built on the major macOS and Linux versions to ensure compatibility.

### NIXOS - Package Manager

[NixOS](https://nixos.org) - is a Linux distribution that emphasizes declarative configuration and reproducible builds. 

NIXOS uses the Nix package manager to ensure that systems are defined in a clear and consistent manner through configuration files. NixOS allows for easy rollback of system changes, promotes reliable system management, and simplifies deployment by creating reproducible environments. It's ideal for developers, sysadmins, and those seeking a highly customizable and maintainable Linux setup.

### APT - Advanced Package Tool

[APT (Advanced Package Tool)](https://manpages.debian.org/bookworm/apt/apt.8.de.html) - "is a package management system used by Debian and its derivatives (like Ubuntu) to handle software installation, upgrades, and removal."

APT simplifies the process of managing packages by automatically resolving dependencies, ensuring that software libraries and components required for installation are also handled. It provides a command-line interface with commands like apt-get and apt-cache for installing, updating, and managing packages, offering an efficient and reliable way to manage software on Debian-based systems.

* [APT History](https://en.wikipedia.org/wiki/APT_(software))

### APK

[APK (Alpine Package Keeper)](https://docs.alpinelinux.org/user-handbook/0.1a/Working/apk.html) -  "is the package manager used by the Alpine Linux distribution"

APK is designed to manage system packages, allowing users to install, upgrade, and remove software efficiently. APK simplifies package management by using a lightweight format, ensuring fast installation and low resource consumption. It is the primary method for installing additional software on Alpine Linux, and is part of the apk-tools package, providing users with a reliable tool for maintaining their system's software.

### Helm

[Helm](https://helm.sh) - "is a package manager for Kubernetes that simplifies the deployment and management of applications and services on Kubernetes clusters."

Helm uses Helm charts, which are predefined templates containing all the necessary resources, configurations, and dependencies for deploying an application. Helm allows for easy installation, versioning, and management of Kubernetes applications, making it simpler to handle complex deployments and rollbacks. By using Helm, teams can ensure consistent, repeatable, and scalable deployments within Kubernetes environments.

### Kustomize

[Kustomize](https://kustomize.io) - "is a tool for managing Kubernetes configurations by enabling customization of YAML files without altering the original source code."

Kustomize allows users to create reusable and maintainable Kubernetes manifests by applying "overlays" on top of base configurations. This helps in managing different environments (e.g., development, staging, production) with minimal duplication. Kustomize integrates directly into kubectl, making it a seamless tool for Kubernetes-native configuration management. It simplifies the management of configurations while keeping them consistent across different deployments.

### PIP

### NPM

### Java JAR/WAR

## Terminals

### ⭐ Kitty

<a href="https://sw.kovidgoyal.net/kitty">Kitty</a> - The fast, feature-rich, GPU based terminal emulator.

* [https://sw.kovidgoyal.net/kitty/graphics-protocol/](Terminal graphics protocol)

### wezterm

<a href="https://wezfurlong.org/wezterm/">wezterm</a>
 - "is  a fast, modern, and feature-rich terminal emulator and multiplexer, written in Rust for cross-platform support."
 
Wezterm offers GPU-accelerated rendering, flexible configuration, and built-in support for features like multiplexing and tabs. Designed for speed and usability, WezTerm works seamlessly on Windows, macOS, and Linux, catering to developers who need a reliable and customizable terminal experience.

### ⭐ iTerm2

<a href="https://iterm2.com">iTerm2</a> - "is a feature-rich terminal emulator for macOS, serving as a modern replacement for the default Terminal app and the successor to iTerm."

iTerm2 is designed for macOS 10.14 or newer, it enhances the terminal experience with advanced features such as split panes, search, autocomplete, and session restoration. iTerm2 is tailored for developers who want a powerful and customizable terminal environment.

### Ghostty

<a href="https://ghostty.org">ghostty</a> - " is a high-performance, cross-platform terminal emulator that leverages GPU acceleration for fast rendering and uses platform-native UI for a seamless experience."

Ghostty is designed for modern developers, it combines speed, advanced features, and intuitive usability, making it a robust choice for diverse development workflows.

### Apple Terminal

<a href="https://support.apple.com/de-de/guide/terminal/welcome/mac">Apple Terminal</a> - "is a powerful command-line interface included with macOS, allowing users to control their computer and execute tasks using text-based commands."

Terminal provides access to Unix-based tools and scripts, enabling advanced customization, system management, and automation. Terminal supports macOS-native features while being a gateway for developers and power users to interact with the operating system at a deeper level.

### Xterm.js

[Xterm.js](https://xtermjs.org) - is an open-source JavaScript library for embedding terminal functionality into web applications. 

Xterm.js provides a highly configurable and feature-rich terminal emulator, supporting features like Unicode, color, mouse events, and customizable themes. Xterm.js is designed to work seamlessly in modern browsers, allowing developers to integrate terminal interfaces within web applications without requiring external plugins. It is widely used in cloud-based environments, code editors, and other web-based tools where terminal interaction is needed.

* [xterm history](https://invisible-island.net/xterm/)

### ⭐ tmux

[tmux](https://github.com/tmux/tmux/wiki) - is a terminal multiplexer that allows users to run multiple terminal sessions within a single window. 

Tmux includes detailed guides on installation, configuration, and usage of tmux, as well as advanced features like session management, window splitting, and custom key bindings. The wiki also offers troubleshooting tips, example workflows, and community contributions to help users leverage tmux for increased productivity in terminal-based environments. It's a valuable resource for both beginners and advanced users looking to optimize their terminal experience.

### tmate

[Tmate](https://tmate.io) - "is a web-based platform that provides instant, secure SSH access to terminal sessions."

Tmate allows users to share terminal sessions in real time, enabling collaborative debugging, pair programming, or training. Tmate generates a unique URL that can be shared with others to grant them access to the terminal session, without requiring any setup or special configurations. It is built on top of tmux, offering a simple way to collaborate on projects or remotely support users, making it a useful tool for teams, educators, and system administrators.

### ⭐ screen

The [GNU Screen](https://www.gnu.org/software/screen/manual/screen.html) - "is a terminal multiplexer that allows users to manage multiple terminal sessions within a single window."

Screen enables features such as session persistence, where terminal sessions continue running in the background even after disconnection, and the ability to split windows for multitasking. It is especially useful for remote work over SSH, allowing users to resume sessions and manage multiple tasks efficiently. The manual includes installation instructions, usage examples, and advanced features to help users maximize productivity with Screen.

## Shells

### sh

### bash

### zsh

### fish

## Documentation As Code

Code and documentation, created and maintained equally. developers love it, as it’s effective and takes the pain out of documentation.

### Docs as Code

[Docs as Code](https://docsascode.org) is an approach to documentation where documentation is treated like code, using similar processes, tools, and workflows.

It emphasizes version control, collaboration, and automation to create, maintain, and update documentation in a systematic, reproducible manner. This approach enables teams to use the same infrastructure they use for software development (e.g., Git, CI/CD pipelines) for their documentation. Docs as Code promotes quality, consistency, and efficiency in producing technical and product documentation. The Docs as Code website provides guidelines, best practices, and resources for adopting this methodology.

### Arc42

[arc42](https://arc42.org) -  "is a framework for documenting software and system architectures."

Arc42 provides a structured approach to capturing and communicating architectural decisions, designs, and rationale. The framework consists of a set of templates and guidelines to ensure comprehensive, consistent documentation. arc42 covers all aspects of software architecture, including system components, deployment, quality attributes, and technical constraints, making it valuable for teams looking to maintain clear and organized architecture documentation throughout a project's lifecycle.

### ADR

"Documenting Architecture Decisions" emphasizes the importance of capturing and documenting architectural decisions made during software development. It suggests that these decisions should be clearly articulated, concise, and accessible to ensure that they are understood and can be referenced later. The post encourages using simple, lightweight formats to document architecture decisions and highlights the value of preserving rationale behind decisions, which helps future development teams understand and maintain the system.

* [Documenting architecture decisions](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions)
* [Architectural Decision Record](https://adr.github.io)
* [adr-tools](https://github.com/npryce/adr-tools)
* [Asciidoc tool ADR](https://unexist.dev/documentation/myself/2024/10/25/decision-records.html)

### RFC

* A [Request for Comments (RFC)](https://en.wikipedia.org/wiki/Request_for_Comments) is a publication in a series from the principal technical development and standards-setting bodies for the Internet, most prominently the Internet Engineering Task Force (IETF).
* [Transparent Cross-Team Decision Making using RFCs](https://patterns.innersourcecommons.org/p/transparent-cross-team-decision-making-using-rfcs)

### Presenterm

[Presenterm](https://mfontanini.github.io/presenterm/) - "is a tool that allows you to create and deliver presentations directly from your terminal using markdown format."

Presenterm supports images, animated GIFs, customizable themes, and code highlighting to enhance presentations. Presenterm also enables exporting presentations into PDF format and includes various other features for a streamlined, command-line-driven presentation experience. It's an ideal choice for developers and tech enthusiasts who prefer working in a terminal environment.

### Reveal.js

[Reveal.js](https://revealjs.com) - "is an open-source HTML presentation framework that allows users to create interactive and visually appealing slide decks."

RevealJS supports a range of features such as slide transitions, markdown support, themes, and even live code editing, making it ideal for developers and presenters. Reveal.js offers full customization with the ability to integrate plugins, animations, and multimedia content. It's browser-based and can be easily shared, making it a versatile tool for creating presentations without relying on proprietary software.

### Hugo

[Hugo](https://gohugo.io) - "is a fast, open-source static site generator designed for building websites and blogs. "

Hugo allows developers to create content-driven sites using simple markdown files, and it offers a range of features, including templates, content management, and easy deployment. Known for its speed and flexibility, Hugo can generate sites in seconds and supports various content formats. It is highly customizable and works well with version control and modern web development workflows, making it a popular choice for developers looking to build fast, scalable static websites.

* [HugoMods](https://hugomods.com)
  * Third party Hugo modules and tools for building fast, modular, modern themes and static websites.
* [Hugo Docker Images](https://docker.hugomods.com)
* [Build an amazing docs site](https://getdoks.org)

### Netlify

[Netlify](https://www.netlify.com) -  "is a platform that simplifies the development, deployment, and hosting of modern web applications."

Netlify offers a seamless workflow for front-end developers, integrating continuous deployment, serverless functions, and content delivery through a global CDN. Netlify supports static sites, dynamic applications, and integrates with popular frameworks like React, Gatsby, and Hugo. With features like form handling, A/B testing, and serverless backend integration, Netlify enables fast and efficient website and application management, making it a popular choice for developers aiming for quick deployment and scalability.

### asciinema

[Asciinema](https://asciinema.org) - "is an open-source platform that allows users to record and share terminal sessions in a lightweight, text-based format."

Asciinema enables developers and users to capture, replay, and share interactive shell sessions, making it easier to demonstrate commands, workflows, or troubleshooting processes. Asciinema recordings are highly compressed and can be embedded into websites, shared via URLs, or stored on the platform for future reference. The tool is popular for creating tutorials, guides, and showcasing technical processes efficiently.

### Formats and Diagrams

* [The Markdown Guide](https://www.markdownguide.org)
* [Asciidoc](https://asciidoc.org)
* [Yaml](https://yaml.org/spec/)
  * [yq](https://mikefarah.gitbook.io/yq) is a lightweight and portable command-line YAML processor.
* [Toml](https://toml.io/en/)
* [Json](https://www.json.org/json-en.html)
  * [jq](https://jqlang.github.io/jq/) is a lightweight and flexible command-line JSON processor.
* [Mermaid](https://mermaid.js.org)
  * [Kubernetes Diagram Guide](https://kubernetes.io/docs/contribute/style/diagram-guide/)
  * [K8s docs mermaid](https://github.com/chrismetz09/K8s-docs-mermaid)
* [plantuml](https://plantuml.com)
  * [Kubernetes-PlantUML](https://github.com/dcasati/kubernetes-PlantUML)
