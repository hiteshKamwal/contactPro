[<Attendance>: 1 : 2024-04-24 09:10:37 (1, 0), <Attendance>: 1 : 2024-04-24 09:10:53 (1, 1), <Attendance>: 1 : 2024-04-24 09:32:38 (1, 0), <Attendance>: 1 : 2024-04-24 09:41:51 (1, 0)]

attendance_data = [
    "<Attendance>: 1 : 2024-04-24 09:10:37 (1, 0)",
    "<Attendance>: 1 : 2024-04-24 09:10:53 (1, 1)",
    "<Attendance>: 2 : 2024-04-24 09:32:38 (1, 0)",
    "<Attendance>: 1 : 2024-04-24 09:41:51 (1, 0)"
]

selected_user_id = 1
selected_punch = 1

# Filter the attendance data based on user_id and punch
filtered_attendance = [attendance for attendance in attendance_data if f"({selected_user_id},{selected_punch})" in attendance]

# Store the filtered data in a variable
selected_attendance = filtered_attendance[0] if filtered_attendance else None

print("Selected attendance:", selected_attendance)
