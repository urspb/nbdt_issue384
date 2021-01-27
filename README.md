# nbdt384
> Test case for nbdev issue #384


## Logbook nbdt_issue384

This test case was assembled on a MacOS system (OS version 10.14.6).

To reproduce my findings, you could follow the steps below:

    pyenv virtualenv 3.7.9 iss384

    git clone https://github.com/urspb/nbdt_issue384.git
    cd nbdt_issue384
    pyenv local iss384
    pip install --upgrade pip
    pip install nbdev
    pip list --local | grep nbdev

    # edit settings.ini
    nbdev_install_git_hooks

## Test #384

For the test of `nbdev_nb2md` please look into `00_core`
