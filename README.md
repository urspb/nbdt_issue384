# nbdt381
> Test case for nbdev issue #381


## Logbook nbdt_issue381

This test case was assembled on a MacOS system (OS version 10.14.6).

To reproduce my findings, you could follow the steps below:

    pyenv virtualenv 3.7.9 iss381

    git clone https://github.com/urspb/nbdt_issue381.git
    cd nbdt_issue381
    pyenv local iss381
    pip install --upgrade pip
    pip install nbdev
    pip list --local | grep nbdev

    # edit settings.ini
    nbdev_install_git_hooks

## Test #381

For the test of `nbdev_nb2md` please look into notebook `00_core`.
