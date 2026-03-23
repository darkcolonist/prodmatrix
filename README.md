# PROD_MATRIX: CSV Day Consolidator

A professional, dark-themed web application designed to consolidate multiple daily performance CSV files into a single, comprehensive "Users x Production" matrix. 

This tool is built to handle inconsistent naming conventions and automatically transposes data so that user performance can be tracked across a monthly cycle at a glance.

## 🚀 Key Features

- **Automated Day Extraction**: Automatically identifies the "Day" of the month from filenames (e.g., `01.csv`, `report_12.csv`).
- **Smart Mapping**: Intelligently detects user and result columns even if headers vary (supports `User`, `Username`, `Name`, `Results`, `Production`, and date-based headers).
- **Sticky Matrix UI**: The leftmost column (Users) stays fixed while scrolling horizontally through days, ensuring data remains readable.
- **Dark Mode Design**: A high-contrast, professional interface built with Tailwind CSS and Lucide icons.
- **Client-Side Processing**: All data is processed locally in your browser; your sensitive CSV data is never uploaded to a server.
- **Export Functionality**: Consolidate and export the final matrix back to a single CSV file.

## 🛠️ Tech Stack

- **React 18** (via CDN)
- **Tailwind CSS** (Styling)
- **Lucide React** (Icons)
- **Babel** (In-browser JSX transformation)

## 📖 How to Use

1. **Upload**: Drag and drop or click to upload multiple daily CSV files.
2. **Review**: The sidebar will list all loaded files and their detected "Day".
3. **Analyze**: Use the main matrix to view performance across the entire period.
4. **Export**: Click the "Export" button to download the consolidated matrix.

## 📂 CSV Requirements

The app is flexible, but for best results:
- **Filenames**: Include the day number in the filename (e.g., `day1.csv` or `01.csv`).
- **Columns**: Files should ideally have two columns. The first for the user identifier and the second for the production value.

## 🌐 Hosting on GitHub Pages

This project is designed as a single-file application, making it perfect for GitHub Pages.

1. Create a new repository on GitHub.
2. Upload `index.html` to the root directory.
3. Go to **Settings > Pages**.
4. Under **Build and deployment > Branch**, select `main` (or `master`) and `/ (root)`.
5. Click **Save**. Your app will be live at `https://<your-username>.github.io/<repo-name>/`.

## 📄 License

This project is open-source and free to use.
