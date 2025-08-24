# 🌦️ Weather Comparison Automation - UiPath Project

This UiPath automation project compares the current weather of two cities using a browser (Microsoft Edge), extracts the temperature and condition, determines which city is hotter, displays the result, and stores the data in an Excel file.

---

## 📁 Project Structure

### 1. **User Input**
- Prompts the user to input the names of two cities (`city1` and `city2`).

### 2. **Weather Lookup via Browser**
- Opens Microsoft Edge.
- Searches for weather in each city using Google search.
- Extracts:
  - Temperature (e.g., `31°C`)
  - Weather condition (e.g., `Partly cloudy`)

### 3. **Data Processing**
- Converts temperature strings to numerical values.
- Compares the temperatures to determine which city is hotter.

### 4. **Display Result**
- Shows a message box with:
<City1>: <Temp1>, <Condition1>
<City2>: <Temp2>, <Condition2>
Hotter City: <hotterCity>



### 5. **Store in Excel**
- Adds the weather data into a data table.
- Writes the data to an Excel file:



---

## 🔧 Technologies Used

- UiPath Studio
- Microsoft Edge
- Excel Workbook Activities
- Google Search

---

## 🗂️ Variables

| Variable     | Type      | Description                            |
|--------------|-----------|----------------------------------------|
| `city1`      | String    | First city entered by the user         |
| `city2`      | String    | Second city entered by the user        |
| `temp1`      | String    | Temperature string of city1 (e.g., "31°C") |
| `temp2`      | String    | Temperature string of city2            |
| `temp1Num`   | Double    | Numeric temperature for city1          |
| `temp2Num`   | Double    | Numeric temperature for city2          |
| `condition1` | String    | Weather condition for city1            |
| `condition2` | String    | Weather condition for city2            |
| `hotterCity` | String    | Name of the hotter city                |
| `weatherTable` | DataTable | Stores cities and temperatures         |

---

## 📥 Output

- Excel file at:
your selected location in drive



- Format:
| City    | Temperature |
|---------|-------------|
| Delhi   | 31          |
| Mumbai  | 33          |

---

## 📝 Prerequisites

- UiPath Studio installed
- Microsoft Edge installed
- Excel activities enabled in UiPath
- Internet access
- Folder: `C:\Users\<YourUsername>\Documents\Weather`

---

## 🚀 How to Run

1. Open the project in UiPath Studio.
2. Run the automation.
3. Enter two cities when prompted.
4. View the weather comparison in a message box and Excel file.

---

## 📄 License

This project is open-source and available under the MIT License.
