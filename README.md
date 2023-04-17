# `sinteractive`

A copy of the existing `sinteractive` script on Cheaha.

This repository is provided temporarily for continuity as we develop solutions
to support researchers with no other recourse.

## Installation

1. Open a terminal on Cheaha.
    - Navigate to <https://rc.uab.edu>.
    - In the top navigation menu, click "Clusters" and then "Cheaha Shell Access".
2. Enter `mkdir ~/bin` to create a directory to store the script.
3. Enter `cd ~/bin` to enter that directory.
4. Enter `git clone https://gitlab.rc.uab.edu/rc-data-science/sinteractive-temporary-for-continuity.git ~/bin/sinteractive` to clone this repository into the folder `~/bin/sinteractive`.
5. Etner `cd sinteractive` to enter the new subfolder.
6. Enter `chmod u+x sinteractive _interactive _interactive_screen` to make the scripts executable.

## Usage

At a terminal, enter `~/bin/sinteractive/sinteractive` along with any flags you require, the same as you would with the system-wide installation of `sinteractive`.

### Optional convenience

**Important**: The following only applies if you choose to not use `module reset`. It is considered best practice to start scripts with `module reset` to ensure a clean environment. Doing so will prevent the following suggestion from working. Instead you will need to use the absolute path to the installed `sinteractive` script.

Optionally, and for convenience, you can add the executable to your `$PATH` variable. Modify your `.bashrc` file to include the following line at the end. We prepend the install directory so that the custom executable is found before the system executable.

```shell
PATH="~/bin/sinteractive${PATH:+:${PATH}}"
```

You can modify your `.bashrc` file using your favorite editor. If you are unfamiliar with editing scripts on Cheaha, please try the following.

1. Navigate to <https://rc.uab.edu>.
2. In the top navigation menu, click "File Browsers" and then "Home Directory".
3. At the top-right of the page that opens, check "Show Dotfiles". See [here](https://docs.rc.uab.edu/cheaha/open_ondemand/ood_files/) for more information.
4. In the central pane, scroll down to find the file `.bashrc` and click it once.
5. Among the action buttons near the top of the page, click "Edit".
6. Add the line given above at the end of the editor window. Ensure the file ends with a blank line!
7. Click the "Save" button at the top-left.
8. Test that it works by opening a new terminal window and entering `which sinteractive`. The first result should be `/home/$USER/bin/sinteractive/sinteractive`.

## Support

If you need assistance with these instructions, please contact us at <support@listserv.uab.edu> or visit our [Office Hours](https://docs.rc.uab.edu/#contact-us).

We are not able to provide support for the script or its functionality. If there are errors or other issues we may be able to help find workarounds or troubleshoot this installation. Please contact us.
