# Inventory

# The idea is to store Rule 'Objects' in database as they can be many 100s.

# A separate application is needed to upload Rule 'Objects' to database.

# The reason for storing rule Objects in database is that they will be
# in hundreds and separate applications can be developed to simulate rules
# on a large number of Item's.
# 
# Each rule implementaion will contain a Predicate to figure out if this
# rule can be applied to it.

# Guava cache is used with expiry time of entries as 2 minutes

# That separate application would be given 'Rule' interface from this application
# to create different implementation classes and storing those objects in database.

# In memory DB h2 is used for testing .
