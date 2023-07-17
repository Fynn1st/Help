# Help
I need Help and I dont really know what im doing here rn
so I want that the code Outputs either two names if you dont put in a middle name, or three names (first,middle and last). But it always prints out 3 but if you input only two it prints out the middle name as nothing 
so if someone maye could help me i litterally dont even know if anybody can see this 

    First_Name = None
    Last_Name = None
    Middle_Name = None

    Full_Name = input("Wie Heißt du? ")             # Get entire input
    print(Full_Name)                                # Test the Input

    Leerzeile = Full_Name.find(" ")                 # Find The end of the First name by finding the space
    #print("Leerzeile: " + str(Leerzeile))
    First_Name = Full_Name[:Leerzeile]              # Defining the first name as the part from beginning to the first space
    Last_Name = Full_Name[Leerzeile + 1:]           # Defining the Last name as everything after the first space

    if Last_Name.find(" ") is None:                 # If there is no second Space Print First And last name
        print(First_Name)
        print(Last_Name)
    elif Last_Name.find(" ") is not None:           # If there is a second space
        Leerzeile2 = Last_Name.find(" ")            # Finding the second space
        print("Leerzeile2: " + str(Leerzeile2))     # Control printing the second Space
        Middle_Name = Last_Name[:Leerzeile2 + 1]    # Defining the middle name as the part befor the second space of the prior last name
        Last_Name = Last_Name[Leerzeile2 + 1:]      # Defining the last name as Everything after the Second space

        print(First_Name)                           # Printing all names
        print(Middle_Name)
        print(Last_Name)

    else:
        print("Error")                             # Error


