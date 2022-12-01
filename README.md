# calculating-number-of-months-in-a-given-months
month = int(input("Enter month  in 'MM' format :"))
year = int(input("Enter Year  in 'YYYY' format :"))
Months = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
if (month>0 and month<=12 and year>0  ):   
    if(month == 1 or month == 3 or month == 5 or month == 7 or month == 8 or month == 10 or month == 12):
        print('Number of days in ',end=" ")
        print( Months[month-1],end=" ")
        print( 'are 31')
    elif((month == 2) and ((year%400==0) or (year%4==0 and year%100!=0))):
        print('Number of days in ',end=" ")
        print( Months[month-1],end=" ")
        print( 'are 29')
    elif(month == 2):
        print('Number of days in ',end=" ")
        print( Months[month-1],end=" ")
        print( 'are 28')
    else:
        print('Number of days in ',end=" ")
        print( Months[month-1],end=" ")
        print( 'are 30')
else:
    print('check your input')
    


      
