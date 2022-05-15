# Icecream-shop
class Icecream(object):
    def __init__(self, name, price):
        self.name = name
        self.price = price
    
    def getprice(self):
        return self.price
    
    def __str__(self):
        return self.name + ' : ' + str(self.getprice())
  
# Defining a function for building a Menu 
# which generates list of Icecreams    
def buildmenu(names, costs):
    menu = []
    for i in range(len(names)):
        menu.append(Icecream(names[i], costs[i]))
    return menu

# items
names = ['stick','cone','cup']

# prices
costs = [20,30,40]

# building Icecream type menu
Icecream = buildmenu(names, costs)

n = 1
for el in Icecream:
    print(n,'. ', el)
    n = n + 1
class flavour(object):
    def __init__(self, name, price):
        self.name = name
        self.price = price
    
    def getprice(self):
        return self.price
    
    def __str__(self):
        return self.name + ' : ' + str(self.getprice())
  
# Defining a function for building a Menu 
# which generates list of flavours Menu 
def build(name1, cost):
    menu = []
    for i in range(len(name1)):
        menu.append(flavour(name1[i], cost[i]))
    return menu

# items
name1 = ['chocolate','vennila','strawberry']

# prices
cost = [20,30,40]

# building flavour menu
flavour = build(name1, cost)

n = 1
for el in flavour:
    print(n,'. ', el)
    n = n + 1
a=input("Type of Icecream is:")
for i in range(len(names)):
    if names[i]==a:
        c=costs[i]
        break
        
else:
    print("we haven't that flavour")
        
b=input("Flavour of Icecream is:")
for i in range(len(name1)):
    if name1[i]==b:
        d=cost[i]
        break
else:
    print("we haven't that type icecream")
quantity=int(input("Enter how many ice creams do you want:"))
print("The bill amount for your icecream:",d+c*quantity)



