# Textbook-Exercises
def elast(price1,amount1,price2,amount2):
  elasticity = (amount2 - amount1) / (price2 - price1)
  return (elasticity)
  
def scale_elast(elasticity):
  if elasticity == 0 : 
    return 'Perfectly Inelastic'
  elif elasticity < 1 :
    return 'Relatively inelastic'
  elif elasticity == 1 : 
    return 'Unit Elastic'
  elif elasticity > 1 : 
    return 'Relatively Elastic'

price1 = float(input('Enter the prior price : '))
amount1 = float(input('Enter the prior amount : '))
price2 = float(input('Enter the latter price : '))
amount2 = float(input('Enter the latter amount : '))

elasticity = elast(price1,amount1,price2,amount2)
print('Elasticity = ',elasticity)

character = scale_elast(elasticity)
print('Character of product = ', character)
