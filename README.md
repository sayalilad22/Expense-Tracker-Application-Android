# Expense Tracker Application

A simple Android application to track and manage daily expenses with category-wise visualization.

## Description

This Android application helps users track their daily expenses efficiently. Users can add, edit, and delete expense records with details like amount, date, notes, and category. The app provides a visual representation of expenses through a pie chart, showing spending distribution across different categories.

### Features

- Add new expenses with amount, date, notes, and category
- Edit existing expense records
- Delete unwanted expenses
- View total expenses at a glance
- Visualize expense distribution by category using an interactive pie chart
- Categorize expenses into: Food, Transport, Shopping, Bills, Entertainment, and Other
- Local data persistence using Room database
- Material Design UI with custom icons for each category

## Technologies Used

- **Language**: Java
- **Platform**: Android SDK
  - Minimum SDK: 24 (Android 7.0)
  - Target SDK: 36
  - Compile SDK: 36
- **Database**: Room Persistence Library (v2.6.1)
- **UI Components**:
  - RecyclerView for expense list
  - Material Design Components (v1.11.0)
  - MPAndroidChart (v3.1.0) for pie chart visualization
- **Build System**: Gradle
- **Additional Libraries**:
  - AndroidX AppCompat
  - Core SplashScreen API

## Project Structure

```
app/src/main/java/com/example/myapplication/
├── MainActivity.java          # Main screen with expense list and pie chart
├── SplashActivity.java        # Splash screen on app launch
├── Expense.java               # Expense entity/model
├── ExpenseDao.java            # Database access object (Room DAO)
├── ExpenseDatabase.java       # Room database configuration
├── AppDatabase.java           # Database builder
├── ExpenseAdapter.java        # RecyclerView adapter for expense list
└── CategoryTotal.java         # Model for category-wise totals
```

## How to Build

### Prerequisites

- Android Studio (latest version recommended)
- JDK 11 or higher
- Android SDK with API level 36

### Build Steps

1. Clone or download this repository
2. Open the project in Android Studio
3. Wait for Gradle sync to complete
4. Build the project:
   - Click on **Build** > **Make Project** or press `Ctrl+F9` (Windows/Linux) or `Cmd+F9` (Mac)
5. Run the application:
   - Connect an Android device or start an emulator
   - Click on **Run** > **Run 'app'** or press `Shift+F10` (Windows/Linux) or `Ctrl+R` (Mac)

### Build via Command Line

```bash
# Build debug APK
./gradlew assembleDebug

# Build release APK
./gradlew assembleRelease

# Install on connected device
./gradlew installDebug
```

The generated APK files will be available in:
- Debug: `app/build/outputs/apk/debug/app-debug.apk`
- Release: `app/build/outputs/apk/release/app-release-unsigned.apk`

## Usage

1. Launch the app
2. Tap the **+** (Floating Action Button) to add a new expense
3. Fill in the expense details (amount, date, note, category)
4. View all expenses in the list below
5. Edit an expense by tapping the edit icon
6. Delete an expense by tapping the delete icon
7. Check the pie chart for category-wise expense distribution

## License

This is a personal project for educational purposes.
