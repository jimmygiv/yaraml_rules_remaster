# YaraML Rules Remaster
This is a super basic overview of how I want to rework YaraML. I know this is a very ambitious project, but I want to try to make this headless or gui. And take this same basic logic and:
* Create a "master" config file for simple tuning
* Rework imports/setup
* Add possibility of importing hex,hexdump, or base64 stored files. Some arent allowed to store malware on-disk due to policy.
* Seperate tuning for different file/magic types
* Grade the generated rules for efficency
  `Rule ran x fast over x num of files, with x/y detection rate. I gib score A+, this cant ever be improved. It is the embodiment of perfection`
* Try to auto-magically simplify some rule syntax as well as detect same character strings with different casing
    `$s\s=\s"SOMESTRING" -> "SOMESTRING".lower() == "sOmEsTrInG".lower()`
* Provide a rough characterization of the file structers taken.
  `IE: Top 10 strings ascii, wide, file min/max, `
![image](https://github.com/jimmygiv/yaraml_rules_remaster/assets/56000678/639671d7-d770-44a7-b4a8-0fec72d20290)
