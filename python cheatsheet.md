Python cheatsheet

### String

concatinate strings like a pro

	foobar = ''.join(['foo', 'bar'])


### variable type

dictionary:

	test = {'name':'John','job':'teacher'}
	print test['job'] # prints teacher

lists

	zoo_animals = ["pangolin", "cassowary", "sloth"];
	zoo_animals.append("ape")
	first = zoo_animals[0:2]   # The first two items;second parm ends -before- index b
	zoo_animals.insert(1,"cobra") #change cassowary to cobra
	zoo_animals.index("cobra") # returns 1


return vars greater then 4

	a = [3, 4, 5]
		b = [i for i in a if i > 4]
	or 
		b = filter(lambda x: x > 4, a)

enumerate a list

	a = [3, 4, 5]
	a = [i + 3 for i in a]
Or:
	a = map(lambda i: i + 3, a)


### functions

#### using functions the right way

def make_complex(x, y):
    return {'x': x, 'y': y} # return a list instead of just a var


