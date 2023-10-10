# fun_bank_uname_password.py
#program
counter=0
def logintry():
    username=input("enetr user name")
    password=input("enter pass word:")
    login(username,password)
def login(uid,pwd):
    global counter
    if uid=="ADMIN" and pwd =="st0re@1":
        print("login successful")
        return
    else:
        counter+=1
        print("the user name or password is incorrecct")
        if  counter>2:
            print("account blocked")
            return
        else:
            print("try again")
            logintry()
#start with thw program by calling function
logintry()
