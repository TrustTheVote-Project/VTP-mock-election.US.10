# A VoteTrackerPlus Mock US Election Repo

This is work in progress - like in a major way.

This repo represents current thoughts on how to configure an election for VoteTrackerPlus.  See the [VoteTrackerPlus](https://github.com/TrustTheVote-Project/VoteTrackerPlus) for more information.

This repo includes the VoteTrackerPlus repo as a git submodule.

## How to clone this and the VoteTrackerPlus repos and setup up the CLI demo

```bash
# clone both repos (https example)
$ git clone --recurse-submodules https://github.com/TrustTheVote-Project/VTP-mock-election.US.10.git

# Make sure there is a compatible python environment - any reasonable python framework can be used.
# See [VTP-mock-election.US.10/VoteTrackerPlus/src/vtp/README.md](https://github.com/TrustTheVote-Project/VoteTrackerPlus/tree/master/src/vtp)
# for creating either a conda or poetry environment

# Using conda (assumes conda/miniconda has been installed and the env vtp.01 has been created)
$ cd VTP-mock-election.US.10/VoteTrackerPlus/src/vtp
$ conda activate vtp.01

# Using poetry (assumes that peotry has been installed)
$ cd VTP-mock-election.US.10/VoteTrackerPlus
$ poetry install
$ poetry shell
$ cd src/vtp

# To setup a mock demo election, run the following:
$ ./setup_vtp_demp.py
```

See the VTP root repo above for more info.
