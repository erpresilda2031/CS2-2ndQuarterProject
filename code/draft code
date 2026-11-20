# simple code, used as an idea for the `Student login project` before making the finalized code located in the `code` file.

import datetime

# Ask for the students name
def student_login():
    fname = input("\nFirst Name: ")
    lname = input("Last Name: ")
    name = print("Name:", fname.strip().title(), lname.strip().title())

# Check of they are late or not
    date = print(datetime.datetime.now().strftime("%B %-d, %Y"))
    now = datetime.datetime.now()
    time = now.time()
    deadline = datetime.time(7, 3, 0)
    start = datetime.time(5, 0, 0)
# Output
    if time <= deadline:
        print("Status: On Time, welcome!")
    elif time < start:
        print("Status: Too Early, please come back later.")
    else:
        print("Status: Tardy, please get an admission slip.")

print("----- STUDENT LOG-IN PROGRAM -----")
student_login()
