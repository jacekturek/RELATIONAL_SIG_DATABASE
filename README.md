# RELATIONAL_SIG_DATABASE
Social signals explained in a database / database design and some data
Signals can have a form of #...
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
