# Handy Container Environments

Solutions to run containers locally and remotely.

See also this [great summary of local container runtimes](https://docs.google.com/spreadsheets/d/1ZT8m4gpvh6xhHYIi4Ui19uHcMpymwFXpTAvd3EcgSm4/edit#gid=0) by Bret Fisher.

### ⭐ Docker Desktop

<a href="https://www.docker.com/products/docker-desktop/">Docker Desktop</a> - "The fastest way to containerize applications."

At the heart of Docker Desktop is a <a href="https://github.com/linuxkit/linuxkit">LinuxKit</a> VM running (good old) Docker Engine and fronted by an (electron?) GUI. This architecture makes it work the same way on Windows, macOS, and Linux. Additionally, Docker Desktop comes bundled with a local Kubernetes cluster and a powerful mechanism of (GUI) extensions.

### Rancher Desktop

<a href="https://github.com/rancher-sandbox/rancher-desktop/">Rancher Desktop</a> - "Container Management and Kubernetes on the Desktop."

Similar to Docker Desktop but with more focus on local Kubernetes clusters (although it can be used with the Kubernetes functionality disabled). Uses <a href="https://github.com/lima-vm/lima">Lima VMs</a> instead of LinuxKit. Can run either Docker Engine or containerd + nerdctl inside of a VM.

### Podman Desktop

<a href="https://github.com/containers/podman-desktop">Podman Desktop</a> - "Manage Podman and other container engines from a single UI and tray."

### 🤑 OrbStack

<a href="https://orbstack.dev/">OrbStack</a> - "Run Docker [containers] and Linux [VMs] on your Mac seamlessly and efficiently." It looks like a Docker Desktop alternative (but probably without the Docker Desktop extensions yet) with a bunch of appealing capabilities: promises to be fast(er), has a native macOS UI app, can run full-blown (and well integrated with the host) Intel and Apple Silicon Linux VMs with the ease of regular containers. Although it does have one big downside - it's not open-source (seems to be free for the time being, but the plans for eventual monetization were announced)."

### Lima

<a href="https://github.com/lima-vm/lima">Lima</a> - "Linux virtual machines, typically on macOS, for running containerd."

Lima runs a virtual machine (QEMU or Apple's Virtualization Framework) with a custom Linux distro inside that has containerd, BuildKit, and nerdctl preinstalled. It gives you close to Docker (Engine) experience on macOS (and Linux), but also the Lima-managed VM can be used on its own, and it's well-integrated with the host, meaning you can run commands in it easily. Like OrbStack, but without the UI and with many more supported host/virtualization options.

### 🧑‍🔬 Colima

<a href="https://github.com/abiosoft/colima">Colima</a> - "Container runtimes on macOS (and Linux) with minimal setup."

Colima stands for "Cotainers in Lima" - the projects extends the standard Lima capabilities (see above) and makes it possible to run Docker Engine and Kubernetes (powered by?) runtimes inside of a Linux virtual machine (createad by Lima) on macOS (and Linux).

### Finch

<a href="https://github.com/runfinch/finch">Finch</a> - "an open source client for container development."

A minimal native client plus an opinionated distribution of other open source components (nerdctl, containerd, BuildKit, Lima). "Finch aims to help promote other projects by making it easy to install and use them, while offering a simple native client to tie it all together."

### minikube

<a href="https://github.com/kubernetes/minikube">minikube</a> - "Run Kubernetes locally."

Despite the name, <a href="https://minikube.sigs.k8s.io/docs/faq/#can-i-start-minikube-without-kubernetes-running">minikube can be used without Kubernetes!</a>. Running `minikube start --container-runtime=docker --no-kubernetes` gives you some sort of a Docker Desktop replacement. It also uses a lightweight VM to run Docker Engine and works perfectly fine on Windows, macOS (`arm` performance is poor though), and Linux.

### 🧑‍🔬 virt

<a href="https://github.com/apinske/virt">virt</a> - "small Linux VM, ready to run containers, for macOS on ARM." Like Lima but for Podman and using the Apple Virtualization.framework instead of QEMU.

### Vagrant + VirtualBox + Docker provisioner

<a href="https://github.com/hashicorp/vagrant">Vagrant</a> - "a tool for building and distributing development environments."

Vagrant is many things, but in particular it can be used as a handy VirtualBox frontend. With just <a href="https://developer.hashicorp.com/vagrant/docs/provisioning/docker">about 5 lines of config</a>, you can get a local VM with Docker Engine inside. Works the same way on Linux, Windows, and macOS, but no `arm` support is possible. Read more - <a href="https://iximiuz.com/en/posts/how-to-setup-development-environment/">Disposable Local Development Environments with Vagrant, Docker, and Arkade</a>.

### Distrobox

<a href="https://github.com/89luca89/distrobox">Distrobox</a> - "Use any linux distribution inside your terminal. Enable both backward and forward compatibility with software and freedom to use whatever distribution you’re more comfortable with."

More like "a simple way to run a Linux distro in a container". Distrobox uses Podman or Docker to create containers using the Linux distribution of your choice. The created container will be tightly integrated with the host, allowing sharing of the HOME directory of the user, external storage, external USB devices and graphical apps (X11/Wayland), and audio.

### nerdctl

<a href="https://github.com/containerd/nerdctl">nerdctl</a> - "contaiNERD CTL - Docker-compatible CLI for containerd, with support for Compose, Rootless, eStargz, OCIcrypt, IPFS, ..."

Not a full-blown container runtime, but worth an honorable mention.
