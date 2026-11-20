import datetime

def student_login():
    # Tracks daily attendance totals for the final report
    total_students = 0
    on_time_count = 0
    slip_required_count = 0

    # Sets the school's official morning opening and late cut-off times
    start = datetime.time(5, 0, 0)      # 5:00 AM
    deadline = datetime.time(7, 30, 0)  # 7:30 AM

    print("==========================================")
    print("       STUDENT LOG-IN PROGRAM")
    print("==========================================")

    # Repeats the login process so multiple students can check in continuously
    while True:
        # Gets and formats the student's full name
        fname = input("\nFirst Name: ").strip().title()
        lname = input("Last Name: ").strip().title()
        
        # Checks if the student missed the previous school day
        absent = input("Were you absent on the previous school day? (yes/no): ").strip().lower()

        # Captures the current system date and exact arrival time
        now = datetime.datetime.now()
        current_time = now.time()

        # Displays the student's login details
        print("\n------------------------------------------")
        print(f"Name:   {fname} {lname}")
        print(f"Date:   {now.strftime('%B %d, %Y')}")
        print(f"Time:   {now.strftime('%I:%M %p')}")

        # Determines if the student is too early, on time, or needs an admission slip
        if current_time < start:
            print("Status: Too Early, please come again later.")
        elif absent in ["yes", "y"]:
            print("Status: Absent Previously — Please get an admission slip.")
            total_students += 1
            slip_required_count += 1
        elif current_time <= deadline:
            print("Status: On Time, welcome!")
            total_students += 1
            on_time_count += 1
        else:
            print("Status: Tardy (Arrived after 7:30 AM) — Please get an admission slip.")
            total_students += 1
            slip_required_count += 1
        print("------------------------------------------")

        # Prompts the user to continue or end the login session
        another = input("\nLog in another student? (yes/no): ").strip().lower()
        if another not in ["yes", "y"]:
            break

    # Prints the overall attendance summary once the session ends
    print("\n==========================================")
    print("         DAILY ATTENDANCE SUMMARY")
    print("==========================================")
    print(f"Total Students Logged In: {total_students}")
    print(f"On Time (Direct to Class): {on_time_count}")
    print(f"Admission Slip Required:  {slip_required_count}")
    print("==========================================")

# Starts the program
student_login()
