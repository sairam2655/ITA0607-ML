**input**
# another cell
import pandas as pd
import numpy as np

data = {
    "Study_Hours": [
        2, 3, 4, 5, 6, 7, 8, 2, 4, 6,
        7, 8, 3, 5, 6, 9, 1, 4, 7, 8
    ],

    "Attendance": [
        45, 50, 55, 65, 70, 80, 90, 40, 60, 75,
        85, 92, 48, 68, 78, 95, 35, 58, 82, 88
    ],

    # 1 = Project completed
    # 0 = Project not completed
    "Project_Done": [
        0, 0, 0, 1, 1, 1, 1, 0, 0, 1,
        1, 1, 0, 1, 1, 1, 0, 1, 1, 1
    ],

    # 1 = Placed
    # 0 = Not placed
    "Placed": [
        0, 0, 0, 0, 1, 1, 1, 0, 0, 1,
        1, 1, 0, 1, 1, 1, 0, 0, 1, 1
    ]
}

df = pd.DataFrame(data)

print("Student Placement Dataset")
print(df)

**output**
Student Placement Dataset
    Study_Hours  Attendance  Project_Done  Placed
0             2          45             0       0
1             3          50             0       0
2             4          55             0       0
3             5          65             1       0
4             6          70             1       1
5             7          80             1       1
6             8          90             1       1
7             2          40             0       0
8             4          60             0       0
9             6          75             1       1
10            7          85             1       1
11            8          92             1       1
12            3          48             0       0
13            5          68             1       1
14            6          78             1       1
15            9          95             1       1
16            1          35             0       0
17            4          58             1       0
18            7          82             1       1
19            8          88             1       1
