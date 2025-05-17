students = {}

def add_student():
    roll = input("Enter Roll Number: ")
    if roll in students:
        print("Student already exists!")
    else:
        name = input("Enter Name: ")
        age = input("Enter Age: ")
        course = input("Enter Course: ")
        students[roll] = {'name': name, 'age': age, 'course': course}
        print("Student added successfully!")

def view_students():
    if not students:
        print("No students found.")
    else:
        print("\n--- Student List ---")
        for roll, info in students.items():
            print(f"Roll: {roll}, Name: {info['name']}, Age: {info['age']}, Course: {info['course']}")

def update_student():
    roll = input("Enter Roll Number to update: ")
    if roll in students:
        print("Enter new details (leave blank to keep old):")
        name = input(f"New Name (current: {students[roll]['name']}): ") or students[roll]['name']
        age = input(f"New Age (current: {students[roll]['age']}): ") or students[roll]['age']
        course = input(f"New Course (current: {students[roll]['course']}): ") or students[roll]['course']
        students[roll] = {'name': name, 'age': age, 'course': course}
        print("Student updated successfully!")
    else:
        print("Student not found!")

def delete_student():
    roll = input("Enter Roll Number to delete: ")
    if roll in students:
        del students[roll]
        print("Student deleted successfully!")
    else:
        print("Student not found!")

def main():
    while True:
        print("\n--- Student Management System ---")
        print("1. Add Student")
        print("2. View Students")
        print("3. Update Student")
        print("4. Delete Student")
        print("5. Exit")
        choice = input("Enter choice: ")
        
        if choice == '1':
            add_student()
        elif choice == '2':
            view_students()
        elif choice == '3':
            update_student()
        elif choice == '4':
            delete_student()
        elif choice == '5':
            print("Exiting... Bye nerd 🤓!")
            break
        else:
            print("Invalid choice. Try again!")

if __name__ == "__main__":
    main()
