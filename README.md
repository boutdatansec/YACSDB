# YACSDB - Yet Another CyberSecurity Database

YACSDB is a publicly database designed to enhance Natural Language Processing in Cybersecurity Domain. 

The first version is [**YACSDB<sub>NER</sub>**](https://github.com/boutdatansec/YACSDB/blob/main/yacsdb_dataset_v1.1.jsonl) - a dataset for Named Entity Recognition based on STIX Domain Objects.

Paper submited to conference to be published.

## JSONL file information

APT reports from MITRE ATT&CK are available on [STIXNet](https://github.com/Mhackiori/STIXnet/blob/main/Dataset/Annotations.json).

JSONs have a dictionary with two keys: 
- data: Information about the report
  - report (string): Report's ID
  - part (integer): Part number of a report
  - text (string): Report's text
- annotations (list): Entities labeled from the text
  - text (string): Entity span
  - labels (list): Labels associated with entity as a string -- only one label per entity in this version
  - start (integer): Index of starting character of the entity
  - end (integer): Index (exclusive) of ending character of the entity

Original report's names and associated ID can be found in the [metadata](https://github.com/boutdatansec/YACSDB/blob/main/dataset_metadata.csv) file. Kudos to [VX-Underground](https://vx-underground.org/).
