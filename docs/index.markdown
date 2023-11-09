---
layout: default
title: "Sourcesync Pro"
---

Accelerate development cycle with [Sourcesync Pro](https://plugins.jetbrains.com/plugin/22318-source-synchronizer-pro?noRedirect=true), a plugin for all **IntelliJ** based products.

[Sourcesync Pro](https://plugins.jetbrains.com/plugin/22318-source-synchronizer-pro?noRedirect=true)'s synchronization, forwarding and comparison capabilities for local vs remote files provide a fast and seamless way of transferring code, binary artifacts and configuration files between local and remote development environments.

Local **VCS changes**, **files** and **directories** can be transferred on the remote infrastructure using the **SCP** or **SSH** protocols.
Other notable features include:

* **password** and **key pair** authentication
* support for **key pairs** with and without *passphrases*
* timestamp preserving
* file filtering
* user-friendly UI with support for IntelliJ's **New UI** feature
* synchronization of single or multi-selection files as well as VCS changes

---

## Sourcesync vs Sourcesync Pro

[Sourcesync](https://plugins.jetbrains.com/plugin/7374-source-synchronizer?noRedirect=true) is still available and under active development as a free and open source variant. [Sourcesync Pro](https://plugins.jetbrains.com/plugin/22318-source-synchronizer-pro?noRedirect=true) has more features and a more streamlined way of transferring code. Checkout the table below for a full feature comparison.

|                            Features                             |        Sourcesync         |              Sourcesync Pro              |
|:---------------------------------------------------------------:|:-------------------------:|:----------------------------------------:|
|                             License                             | **Free** & **opensource** |  Starts at **$5.99 USD per user/month**  |
|                         SCP File Upload                         |            Yes            |                   Yes                    |
|                        SCP Folder Upload                        |          **No**           |          Yes - Recursive Upload          |
|                      SSH/SFTP File Upload                       |            Yes            |                   Yes                    |
|                     SSH/SFTP Folder Upload                      |          **No**           |          Yes - Recursive Upload          |
|                   Auto Transfer On File Save                    |          **No**           |                   Yes                    |
|           Support For Comparing Local vs Remote Files           |          **No**           |                   Yes                    |
|                 SCP/SSH Password Authentication                 |            Yes            |                   Yes                    |
|    SCP/SSH Key-Pair Authentication With & Without Passphrase    |            Yes            |                   Yes                    |
|                  SCP/SSH timestamp preserving                   |     Modification Time     | Permissions, Access & Modification times |
|                         File Filtering                          |            Yes            |                   Yes                    |
| User-friendly UI with support for IntelliJ's **New UI** feature |            Yes            |                   Yes                    |
|                 Customizable keyboard shortcuts                 |            Yes            |                   Yes                    |
|                       VCS Changes Upload                        |            Yes            |                   Yes                    |
|                   Multi-selection File Upload                   |            Yes            |                   Yes                    |
|                  Multi-selection Folder Upload                  |          **No**           |                   Yes                    |
|                       Editor File Upload                        |            Yes            |                   Yes                    |

---

## FAQ

1. Where are my files transferred?

   Files are transferred on the remote host selected as the main target in the **Sourcesync Configurations** combo box. [Sourcesync Pro](https://plugins.jetbrains.com/plugin/22318-source-synchronizer-pro?noRedirect=true) keeps the remote project structure similar
   to the local one, except the project's base path which will be replaced on the remote target with the **Workspace** configuration value.

   For example, say the **Workspace** remote path is configured to `/home/ifaur/workspace`, and your local project is placed in `C:\\Users\\ifaur\\IdeaProjects\\my-awesome-project`
   then a local file placed in `src\\main\\kotlin\\com\\mypackage\\MyFile.kt` will be transferred to `/home/ifaur/workspace/my-awesome-project/src/main/kotlin/com/mypackage/MyFile.kt`

2. Where are the sync configurations stored?

   [Sourcesync Pro](https://plugins.jetbrains.com/plugin/22318-source-synchronizer-pro?noRedirect=true) keeps sync configurations per project, and it stores its data in the project's `.idea/sourcesyncpro.xml`

3. Where are passwords and certificate passphrases stored?

   [Sourcesync Pro](https://plugins.jetbrains.com/plugin/22318-source-synchronizer-pro?noRedirect=true) makes use of IntelliJ's own credential store framework to securely save sensitive data. **IntelliJ IDEA** does not have its own password store. It uses either the native password management system or KeePass.

4. There are errors when trying to load or persist sync configurations. What do I do next?

   You can simply remove `.idea/sourcesyncpro.xml` from the project's folder and restart IntelliJ. You will have to reconfigure your sync targets.

5. Is [Sourcesync](https://plugins.jetbrains.com/plugin/7374-source-synchronizer?noRedirect=true) still maintained?

   Yes, [Sourcesync](https://plugins.jetbrains.com/plugin/7374-source-synchronizer?noRedirect=true) is still under active development, it will continue to be a free and open source version. Hoewever the more adavanced features will be found only in [Sourcesync Pro](https://plugins.jetbrains.com/plugin/22318-source-synchronizer-pro?noRedirect=true).

---

## Issues

Bugs can be reported at https://github.com/fioan89/sourcesync/issues please add the `[Pro]` in the summary.

---
