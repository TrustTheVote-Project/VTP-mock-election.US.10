# A VoteTrackerPlus Mock US Election Repo

This is work in progress - like in a major way.

This repo represents current thoughts on how to configure an election for VoteTrackerPlus.  See the [VoteTrackerPlus](https://github.com/TrustTheVote-Project/VoteTrackerPlus) for more information.

This repo includes the VoteTrackerPlus repo as a git submodule.

## How to stitch this repo into VTP-root-repo

```bash
# clone both repos
$ git clone --recurse-submodules git@github.com:TrustTheVote-Project/VTP-mock-election.US.10.git

# Make sure there is a compatible python environment - any reasonable python framework can be used.
# See the VTP-mock-election.US.10/VoteTrackerPlus/src/vtp/README.md file for more details.
$ conda activate vtp.01

# To setup a mock demo election, run the following:
$ cd VTP-mock-election.US.10/VoteTrackerPlus/src/vtp
$ ./setup_vtp_demp.py
```

See the VTP root repo above for more info.
