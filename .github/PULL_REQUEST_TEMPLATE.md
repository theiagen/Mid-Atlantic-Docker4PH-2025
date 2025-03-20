<!--
Please replace all '[ ]' with '[X]' to demonstrate completion.
-->

Pull Request (PR) checklist:
- [ ] Include a description of what is in this pull request in this message.
- [ ] The dockerfile successfully builds to a test target for the user creating the PR. (i.e. `docker build --tag samtools:1.15test --target test docker-builds/samtools/1.15` )
- [ ] Directory structure as name of the tool in lower case with special characters removed with a subdirectory of the version number (i.e. `spades/3.12.0/Dockerfile`)
   - [ ] (optional) All test files are located in same directory as the Dockerfile (i.e. `shigatyper/2.0.1/test.sh`)
- [ ] Create a simple container-specific [README.md](../docker/example/README.md) in the same directory as the Dockerfile (i.e. `spades/3.12.0/README.md`)
   - [ ] If this README is longer than 30 lines, there is an explanation as to why more detail was needed
- [ ] Dockerfile includes the recommended [LABELS](../docker/example/Dockerfile#L22-L31) 
- [ ] Main [README.md](../README.md) has been updated to include the tool and/or version of the dockerfile(s) in this PR