# Server Health Checker Bot 🤖

A UiPath RPA bot that automatically checks the availability of servers/URLs and logs their status in real time.

## 📌 Business Value
Manual server monitoring is time-consuming and error-prone. This bot automates the process — checking multiple servers in seconds and logging results with timestamps, freeing up IT teams for higher-value work.

## ⚙️ How It Works
1. Reads a list of URLs from an Excel file (ServerList.xlsx)
2. Sends an HTTP Request to each URL
3. Captures the response status (OK, ServiceUnavailable, etc.)
4. Logs the result with timestamp in the Output panel

## 🛠️ Tech Stack
- UiPath Studio
- UiPath HTTP Request Activity
- Excel (ServerList.xlsx as input)
- UiPath Orchestrator (Community Cloud)

## 📂 Project Structure

CheckServerStatus/
├── Main.xaml          — Main workflow
├── ServerList.xlsx    — Input file with URLs to check
├── project.json       — UiPath project configuration

## 🚀 How To Run
1. Clone this repository
2. Open Main.xaml in UiPath Studio
3. Add your URLs to ServerList.xlsx under the "URL" column
4. Press F5 to run
5. Check Output panel for server status results

## 📊 Sample Output
| URL | Status |
|---|---|
| https://www.google.com | OK |
| https://www.github.com | OK |
| https://www.thiswebsitedoesnotexist123.com | ServiceUnavailable |

## 👨‍💻 Author
Dhiliphen — Senior RPA Developer with 5+ years of enterprise automation experience.
[LinkedIn](https://linkedin.com/in/dhiliphen) | [GitHub](https://github.com/dhiliphen)
