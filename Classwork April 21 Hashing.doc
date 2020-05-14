import hashlib

import item as item

items = [25, 54, 34, 67, 75, 21, 77, 31, 4]


def hash(item_list, table_size):
    hash_table = dict([(i, None) for i, x in enumerate(range(table_size))])
    for item in item_list:
        i = item % table_size
        if bool(hash_table[i]):
            i = 1 + i
            hash_table[i] = item
            print("The hash for %s is %s" % (item, i))
        else:
            print("The hash for %s is %s" % (item, i))
            hash_table[i] = item

    return hash_table


# Execute the hash function # Create table with 11 entries to match example above
hash_table = hash(items, 12)

# Print the resulting hash table
print(hash_table)

# testing
print(bool(items[1]))
i = 2
print(bool(items[i]))


# https://edhenry.github.io/2016/12/21/Hashing-in-Python/
# https://www.programiz.com/python-programming/methods/built-in/hash