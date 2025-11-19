# SecOps-AnalyticsRules

All rulesets, regardless of language, should be stored centrally in this repo.

These can be used ad hoc, such as in the case of YARA, or added to analytic rule schedules, like KQL, in Sentinel.

Regardless, any rule that is run and has any value, should be added to the repo for use by any member of the team.

# KQL
KQL rules are primary run against Sentinel or MS Defender.
These can be run as rules, inside workbooks or as ad hoc queries.
No rules are to be added to the Defender detection rules. Where a detection rule is required
it is to be run as a Sentinel Analytics rule, and appended with "INT - *rulename*".
Ad hoc queries can be run against Sentinel or Defender, however, with Microsoft unifying 
these two systems, it is easier to run them directly in Defender.
Workbooks still require creating and editing in Sentinel, but can be monitored from within
Defender. This should also be merging soon.

# YARA

# Sigma

# VQL