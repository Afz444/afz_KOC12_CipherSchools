# afz_KOC12_CipherSchools
name="Mr John"
balance = 10000
print("----Welcome to Times Bank----")
print("1. Withdraw Money")
print("2. Deposit Money")
print("3. Display Name and Balance")
print("4. Exit/Quit")
choiceNumber = input("Select your choice number from the above menu : ")
if choiceNumber == "1":
    withdrawal = eval(input("Input value to Withdraw : "))
    if withdrawal > balance:
        print("!!!Insufficient Balance!!! ")
        print("Your Current Balance:",balance,"-/Rs")
    else:
        balance = balance - withdrawal
        print("----Withdraw Successfull!----")
        print("Your New Balance: ", balance,"-/Rs")
        if balance <5000:
            print("WARNING!:you are low on balance")
elif choiceNumber == "2":
    deposition = eval(input("Enter the value you want to deposit : "))
    balance = balance + deposition
    print("----Deposition successful!----")
    print("Your New Balance: ", balance,"-/Rs ")
    if balance <5000:
            print("WARNING!:you are low on balance")
elif choiceNumber == "3":
    print("-->Name: ",name)
    print("-->Balance:",balance,"-/Rs")
elif choiceNumber == "4":
    print("Thank you for using our banking system!")
    print("Come again")
    print("Bye bye")
else:
    print("Invalid option selected by the customer")
    print("Please try again later!")
