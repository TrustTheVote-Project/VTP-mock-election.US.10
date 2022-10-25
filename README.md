# A VoteTrackerPlus Mock US Election Repo

This is a work in progress.

This repository represents the current thoughts on how to configure an election for VoteTrackerPlus.  See the [VoteTrackerPlus](https://github.com/TrustTheVote-Project/VoteTrackerPlus) repository for more information.  The VoteTrackerPlus repo is included as a git submodule by this repo.

## How to clone this and the VoteTrackerPlus repos and setup up a VTP demo

Make sure there is a compatible python environment - any reasonable python framework can be used.  See [VTP-mock-election.US.10/VoteTrackerPlus/src/vtp/README.md](https://github.com/TrustTheVote-Project/VoteTrackerPlus/tree/master/src/vtp) for creating either a conda or poetry environment.

```bash
# clone both repos (https example)
$ git clone --recurse-submodules https://github.com/TrustTheVote-Project/VTP-mock-election.US.10.git

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
