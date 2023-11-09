1. Launch the IDE and install the plugin.
2. Restart the IDE.
3. Configure one or more remote sync configurations to target the remote environment where
   you would like to transfer your changes. To create or edit your sync configurations you would have to:
   1. locate the **Sourcesync Configurations** combo box in the IntelliJ's main toolbar panel.

   ![sync_selector_on_main_toolbar](https://raw.githubusercontent.com/fioan89/sourcesyncpro/main/assets/1-sourcesync-configurations-combo-box.png)

   2. Click the combo box drop down icon and then hit the **Edit Sourcesync Configurations** button.
   3. In the new **Sourcesync Remote Configurations** dialog, click **+** on the toolbar or press `Alt + Insert`.
      The list shows the **SCP&SSH** templates available for configuration.

   ![sync_configuration_dialog](https://raw.githubusercontent.com/fioan89/sourcesyncpro/main/assets/2-sorucesync-remote-configurations-dialog.png)

   4. Specify the sync configuration name in the **Name** field. This name will be shown in the list of the available sync configurations.
   5. Fill in the connection details like host, username and password or certificate, depending on the desired authentication type.
   6. Specify the remote base path (excluding the project name) where your files will be transferred.
   7. Apply the changes and close the dialog.
4. From the **Sourcesync Configurations** combo box select a sync configuration as primary target

![sync_configuration_selector](https://raw.githubusercontent.com/fioan89/sourcesyncpro/main/assets/3-sourcesync-configurations-selector.png)

5. Select one or more files, right click, and in the context menu select **Sync selected files to target name**. Alternatively, press `Ctrl + Shift + F2`
6. Alternatively only the file under edit (focused editor) could be transferred by right click in the editor, and in the context
   menu select **Sync this file to target name** or just press `Ctrl + Shift + F1`
7. A third option is to sync all **Git** changed files by right click in the editor or **Project** toolbar, and then select **Sync changed files to target name**. Alternatively, press `Ctrl + Shift + F3`
