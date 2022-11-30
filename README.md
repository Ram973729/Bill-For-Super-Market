# Bill-For-Super-Market
car=60#carrot (Price for 1kg)
pot=50#potato (Price for 1kg)
tom=15#tomato (Price for 1kg)
oni=35#onion  (Price for 1kg)
rad=25#radish (Price for 1kg)
name=input('Enter CustomerName:')
phno=int(input('Enter PhoneNumber:'))
addr=input('Enter Address:')
print('Enter how many kgs do you need for each item')
c=float(input('Carrot:'))#if you want grams then type in decimal number like 0.5 for 500gms.
p=float(input('Potato:'))
t=float(input('Tomato:'))
o=float(input('Onion:'))
r=float(input('Radish:'))
bill=(car*c)+(pot*p)+(tom*t)+(oni*o)+(rad*r)
if bill>3000:
    tax=bill*5/100
elif bill>2000:
    tax=bill*7/100
elif bill>1000:
    tax=bill*10/100
elif bill>500:
    tax=bill*15/100
else:
    tax=100
print('Customer Name:',name)
print('Customer Phno:',phno)
print('Customer Address:',addr)
print('Tax is',tax)
bill=tax+bill
print('Total Amount is',bill)
