# A VoteTrackerPlus Mock US Election Repo

This is work in progress - like in a major way.

This repo represents current thoughts on how to configure an election for VoteTrackerPlus.  See the [VTP-root-repo](https://github.com/TrustTheVote-Project/VTP-root-repo) for more information.

This repo is currently stitched into the VTP-root-repo via a symlink as opposed to a git submodule simply because doing so is just faster and easier at this point.  Once more stuff is working and has been framed out, the symlink will need to be converted to a submodule.

## How to stitch this repo into VTP-root-repo

```bash
# clone both repos
$ git clone git@github.com:TrustTheVote-Project/VTP-root-repo.git
$ git clone git@github.com:TrustTheVote-Project/VTP-mock-election.US.09.git
$ cd VTP-root-repo
$ ln -s ../VTP-mock-election.US.09 ElectionData

# Make sure there is a compatible python environment - any reasonable
# python framework can be used.  See the VTP-root-repo:./bin/README.md file
# for more details.
$ conda activate vtp.01

# To setup a mock demo election, run the following:
$ cd bin
$ ./setup_vtp_demp.py
```

See the VTP root repo above for more info.
