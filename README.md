# 🩺 BMI Health App | C++

A menu-driven health assessment application developed using C++. The application calculates Body Mass Index (BMI), estimates daily calorie requirements, and provides personalized exercise, macronutrient, and meal plan suggestions based on user inputs.

It also supports saving consultation reports to a text file and viewing previously saved reports.

## ✨ Features

- **BMI Calculator:** Calculates BMI using height and weight.
- **BMI Categorization:** Classifies BMI as Underweight, Normal, Overweight, or Obese.
- **BMI Progress Bar:** Displays a visual representation of BMI on a scale from 0 to 40.
- **Calorie Recommendation:** Estimates daily maintenance calories using the Mifflin-St Jeor equation and activity multipliers.
- **Exercise Suggestions:** Provides exercise recommendations based on BMI category and activity level.
- **Macronutrient Breakdown:** Estimates daily protein, fat, and carbohydrate quantities.
- **Sample Meal Plans:** Suggests meal options based on BMI category.
- **Consultation Reports:** Saves the user's name, BMI, and BMI category to a text file.
- **Report History:** Allows users to view previously saved reports.
- **Input Validation:** Handles invalid numeric inputs, empty names, and out-of-range age and activity values.

## 🛠️ Technologies Used

- **C++**
- Standard Template Library (STL)
- File Handling (`fstream`)
- Input Validation (`limits`)
- Mathematical Operations (`cmath`)
- Date and Time Handling (`ctime`)
- String Manipulation (`string` and `cctype`)

## 📋 Prerequisites

Before running the application, ensure you have:

- A C++ compiler such as GCC or MinGW.
- A terminal or command prompt.
- Basic familiarity with compiling and executing C++ programs.

## 🚀 Installation and Setup

### 1. Clone the repository

```bash
git clone NutriTrack
```

Navigate to the project directory:

```bash
cd NutriTrack
```

### 2. Compile the program

Save the source code as `NutriTrack.cpp`.

Using GCC or MinGW:

```bash
g++ NutriTrack.cpp -o NutriTrack
```

### 3. Run the application

**Windows:**

```powershell
.\NutriTrack.exe
```

**Linux/macOS:**

```bash
./NutriTrack
```

## 💻 Application Menu

When the program starts, the following menu appears:

```text
--- BMI Health App ---
1) New consultation
2) View saved reports
3) Exit
```

Choose an option to continue:

- **Option 1:** Start a new health consultation.
- **Option 2:** View previously saved consultation reports.
- **Option 3:** Exit the application.

## 🧮 BMI Calculation

The application calculates BMI using the following formula:

```text
BMI = Weight (kg) / Height (m)²
```

### BMI Categories

| BMI Range | Category |
|---|---|
| Below 18.5 | Underweight |
| 18.5 to below 25 | Normal |
| 25 to below 30 | Overweight |
| 30 and above | Obese |

The application displays the calculated BMI, its category, a progress bar, and a corresponding general recommendation.

## 🔥 Calorie Recommendation

The application estimates Basal Metabolic Rate (BMR) using the Mifflin-St Jeor equation.

**For males:**

```text
BMR = 10 × Weight (kg) + 6.25 × Height (cm)
      - 5 × Age + 5
```

**For females:**

```text
BMR = 10 × Weight (kg) + 6.25 × Height (cm)
      - 5 × Age - 161
```

The estimated daily maintenance calories are calculated as:

```text
Daily Calories = BMR × Activity Multiplier
```

| Activity Level | Multiplier |
|---|---:|
| Low | 1.20 |
| Medium | 1.55 |
| High | 1.725 |

These values are estimates rather than individualized medical prescriptions.

## 🥗 Nutrition and Exercise Suggestions

Based on the calculated BMI category, the application can provide:

**Exercise Suggestions**
- Strength training for underweight users.
- A combination of cardio and strength exercises for normal BMI.
- Cardio-focused activities for overweight and obese categories.
- Additional guidance based on the selected activity level.

**Macronutrient Suggestions**
- Protein: 1.8 grams per kilogram of body weight.
- Fat: 25% of estimated daily calories.
- Carbohydrates: Calculated from the remaining calories after accounting for protein and fat.

**Sample Meal Plans**
- Underweight: Oats, milk, nuts, protein-rich meals, and snacks.
- Normal: Balanced meals containing protein, vegetables, and whole grains.
- Overweight or obese: Sample meals featuring oats, fruit, vegetables, and lean protein.

These are basic program-generated suggestions, not personalized dietary advice.

## 📁 Project Structure

```text
BMI-Health-App/
│
├── NutriTrack.cpp   # Main C++ source code
├── bmi_reports.txt      # Generated consultation reports
└── README.md            # Project documentation
```

The `bmi_reports.txt` file is created when the application saves its first report, provided the file can be opened successfully.

Each report records the consultation date and time, user's name, BMI, and BMI category.

## 🧠 Concepts Demonstrated

This project demonstrates practical applications of:

- Functions and modular programming.
- Conditional statements and loops.
- Input validation and error handling.
- Mathematical calculations.
- String processing.
- File reading and writing.
- Date and time handling.
- Menu-driven console application design.

## 🔮 Future Improvements

- Add a graphical user interface.
- Store complete consultation details in each report.
- Introduce report search and deletion functionality.
- Add more detailed health and fitness tracking.
- Improve nutrition recommendations using additional user information.
- Provide clearer input validation for unrealistic height and weight values.
- Export consultation reports to PDF.

## ⚠️ Disclaimer

This application is intended for educational purposes and general health awareness. BMI and calorie estimates have limitations and should not be treated as medical diagnoses or prescriptions. Consult a qualified healthcare professional for individualized health advice.

## 👩‍💻 Author

**NATARAJA SUNDARI K S**

Developed as a C++ learning project exploring health calculations, input validation, and file handling.
