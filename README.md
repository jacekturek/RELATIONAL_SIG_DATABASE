# RELATIONAL_SIG_DATABASE
# SOCIAL SIGNALS FOR SEO
Social signals explained in a database / database design and some data
Signals can have a form of #...
##
Databases (realtional) are designed hierarchically.
Here I outline TABLES, RELATIONS, ...
##
Tables:
#
Signal:
attributes: signal code(char(5), cheated (bool))
#
Who:
attributes: description (char(25)), where(char(30))
#
Relations:
Signal - 1...* - Who
#
Where from the signal:
attributes: who(description), where (char(30))
#
Relations:
Who 1 - 1 Where from the signal
