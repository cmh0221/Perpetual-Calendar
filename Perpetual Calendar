yu=[0,0,0,0,0,0,0,0,0,0,0,0,0]
year=input('请输入年份（1900年以后）：')
if year[-1]=='年':
    year=year[0:-1]
year=int(year)
print('\t           '*2+str(year)+'年日历',end='\n\n')
def shuchu(month,day):
    print('\t  '*3+str(month)+'月',end='\n\n')
    print('Mon\tTues\tWed\tThur\tFri\tSat\tSun\t')
    for k in yu:
        s=sum(yu)
    print('\t'*(s%7),end='')
    yu[month]=(yu[month]+day)%7
    for i in range(1,day+1):
        print(i,end='\t')
        if (i+s)%7==0:
            print()
    print('\n\n')
def count(month,day):
    yu[month]=(yu[month]+day)%7
def add():
    for y in range(1900,year):
        for month in range(1,13):
            if month in [1,3,5,7,8,10,12]:
                day=31
                count(month,day)
            if month in [4,6,9,11]:
                day=30
                count(month,day)
            if month==2:
                day=28
                if y%4==0:
                    day=29
                if y%100==0:
                    day=28
                if y%400==0:
                    day=29
                count(month,day)
def main():
    add()
    for month in range(1,13):
        if month in [1,3,5,7,8,10,12]:
            day=31
            shuchu(month,day)
        if month in [4,6,9,11]:
            day=30
            shuchu(month,day)
        if month==2:
            day=28
            if year%4==0:
                day=29
            if year%100==0:
                day=28
            if year%400==0:
                day=29
            shuchu(month,day)
main()

