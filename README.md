# Markdown to Google Docs Automator

A modular Python tool designed for **Google Colab** that programmatically converts Markdown meeting notes into a well-formatted Google Document using the Google Docs API.



## 🚀 Key Features

* **Self-Contained Authentication**: Google OAuth logic is built into the main function for a seamless "Run and Auth" experience in Colab.
* **Intelligent Formatting**: 
    * **Headings**: Automatically maps `#`, `##`, and `###` to standard Google Doc Heading styles.
    * **Checkboxes**: Converts Markdown `- [ ]` into interactive, clickable Google Doc checkboxes.
    * **Nested Lists**: Maintains hierarchy and indentation for complex meeting agendas.
* **Member Highlights**: Scans for `@name` mentions and applies **bold blue** styling automatically.
* **Section Breaks**: Converts `---` separators into visual spacing.

---

## 🛠️ Setup & Requirements

### Required Dependencies
The script uses the following libraries:
* `google-api-python-client`
* `google-auth`
* `re` (Regular Expression module)

### Environment
This script is designed specifically for **Google Colab**, which provides pre-installed Google client libraries and native browser authentication support.

---

## 📖 How to Run

### Method 1: The "Open in Colab" Button
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kira2406/AnsibleHealth/ansible_health_task.ipynb)


### Method 2: Open Notebook in Google Colab
1. Download the `ansible_health_task.ipynb` from this repository.
2. Go to [Google Colab](https://colab.research.google.com/).
3. Click **File > Upload notebook** and select the `.ipynb` file.
4. Run all the cells.
5. **Authorize**: A pop-up will appear. Sign in with your Google account to allow the script to create the document in your Drive.
