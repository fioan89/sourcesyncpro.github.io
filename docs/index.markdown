---
layout: default
title: "Sourcesync Pro"
---

Accelerate development cycle with **Sourcesync Pro**, a plugin for all **IntelliJ** based products.

**Sourcesync Pro**'s synchronization and forwarding capabilities provide a fast and seamless way of transfering code, binary artifacts and configuration files between local and remote development environments.

Local changes can be transferred on the remote infrastructure using the **SCP** or **SSH** protocols.
Other notable features include:

- **password** and **key pair** authentication
- support for **key pairs** with and without _passphrases_
- timestamp preserving
- file filtering
- user-friendly UI with support for IntelliJ's **New UI** feature
- synchronization of single or multi-selection files as well as VCS changes

---

## FAQ

1. Where are my files transferred?

   Files are transferred on the remote host selected as the main target in the **Sourcesync Configurations** combo box. **Sourcesync** keeps the remote project structure similar
   to the local one, except the project's base path which will be replaced on the remote target with the **Workspace** configuration value.

   For example, say the **Workspace** remote path is configured to `/home/ifaur/workspace`, and your local project is placed in `C:\\Users\\ifaur\\IdeaProjects\\my-awesome-project`
   then a local file placed in `src\\main\\kotlin\\com\\mypackage\\MyFile.kt` will be transferred to `/home/ifaur/workspace/my-awesome-project/src/main/kotlin/com/mypackage/MyFile.kt`

2. Where are the sync configurations stored?

   **Sourcesync** keeps sync configurations per project, and it stores its data in the project's `.idea/sourcesync.xml`

3. Where are passwords and certificate passphrases stored?

   **Sourcesync** makes use of IntelliJ's own credential store framework to securely save sensitive data. **IntelliJ IDEA** does not have its own password store. It uses either the native password management system or KeePass.

4. There are errors when trying to load or persist sync configurations. What do I do next?

   You can simply remove `.idea/sourcesync.xml` from the project's folder and restart IntelliJ. You will have to reconfigure your sync targets.

---
