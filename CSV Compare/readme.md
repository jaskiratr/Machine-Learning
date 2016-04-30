#### Comparing two CSV files for changes using Pandas for Python
**The changes are reflected in the final dataframe which can be saved 

The changes are reflected in merged differences dataframe. A new column 'changes' is added to describe the changes.

- NaN = = no change

- 1 = updated (2 copies will exist: 0 = old value, 1 = new value)

- -1 = added

- 0 = removed