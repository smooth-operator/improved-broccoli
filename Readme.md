Test repo for filecoin polling tool

Issues added will be converted to polls, if they respect the following template:

```
POLL_DESCRIPTION

---
 Options:
- **< OPTION_LABEL >**: < OPTION_DESCRIPTION >
- **< OPTION_LABEL >**: < OPTION_DESCRIPTION >

---
start: YYYY-MM-DD HH:MM
end: YYYY-MM-DD HH:MM
constituents: [ all | countInMultipleGroups | tokenholders | storageminers | ecosystempartners | appdevs | coredevs | storageclients ]'
```

Options represent the vote options for the poll. Each option has a label and a description. We automatically add an `Abstain` option to the list.
In the constituent groups config, you have 2 special keywords. `all` specifies that all constituent groups are used and `countInMultipleGroups` which controls if a vote in a list based group is counted in the Token Holders group and Storage Miners as well. The other keywords are constituent group names and are self explanatory.

Start and end dates are timestamps in UTC.
