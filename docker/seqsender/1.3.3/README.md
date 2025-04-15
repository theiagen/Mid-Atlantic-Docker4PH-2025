# SeqSender

Main tool: [SeqSender](https://github.com/CDCgov/seqsender)

Public Database Submission Pipeline by CDC

## Example commands

```bash
# Create test submission files with supplied Influenza data
docker run --rm -u $(id -u):$(id -g) -v ${PWD}:/data seqsender:1.3.3 seqsender.py test_data -bsng --organism FLU --submission_dir test_dir

# Create test submission files with supplied SARS-CoV-2 data
docker run --rm -u $(id -u):$(id -g) -v ${PWD}:/data seqsender:1.3.3 seqsender.py test_data -bsng --organism COV --submission_dir test_dir
```

View full `seqsender` help options: `docker run --rm -u $(id -u):$(id -g) -v ${PWD}:/data seqsender:1.3.3 seqsender.py --help`