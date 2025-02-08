# Browser-Based WhatsApp Chat Transcripts (.zip or .txt) to PDF Converter

A simple, client-side tool that converts your WhatsApp chat transcripts into a printable (and PDF-friendly) format. This converter not only renders your chats in a clean, easy-to-read layout but also provides filtering options and interesting statistics.

## Key Features

- **Transcript Parsing:**  
  Converts your WhatsApp text transcripts (copied or uploaded) into a formatted chat view.

- **Markdown & Syntax Highlighting:**  
  Makes use of [Marked](https://github.com/markedjs/marked) and [Highlight.js](https://highlightjs.org/) to support Markdown formatting and code block highlighting within messages.

- **Filtering Options:**  
  Easily filter messages by sender and date range to view specific portions of the chat.

- **Chat Statistics:**  
  Automatically generates statistics including:
  - Total number of messages.
  - Message counts per sender.
  - Chat duration (in days).
  - Longest chat streak. 
  - Monthly distribution of messages displayed as a bar chart (using [Chart.js](https://www.chartjs.org/)).

- **Print to PDF:**  
  Use your browser's print functionality to save the rendered chat transcript (with statistics) as a PDF file.

- **File Upload Support:**  
  In addition to pasting the transcript into the text area, you can also upload a `.txt` file containing your WhatsApp chat transcript.

## How to Use

1. **Open the Converter:**
   - Head to [this link](https://iasad12.github.io/whatsapptranscripttopdf/) to open the converter in any prowser of your choice. 

2. **Input Your Transcript:**
   - **Paste:** Copy your WhatsApp transcript and paste it into the provided text area.
   - **Upload:** Alternatively, click on the file input button to select a `.zip` or `.txt` file containing your chat transcript.

3. **Convert the Transcript:**
   - Click on the **"Render Transcript"** button.
   - The tool will parse the transcript and render the messages in a styled chat view.

4. **Filter Messages (Optional):**
   - Use the filter controls to select a specific sender or narrow down messages by start and end dates.
   - Click **"Apply Filters"** to update the view accordingly.

5. **View Statistics:**
   - The chat statistics section displays the total number of messages and message breakdown by sender.
   - A bar chart visualizes the number of messages per month.

6. **Print or Save as PDF:**
   - When you’re ready to export, click on the **"Print"** button.
   - In the print dialog, choose the option to save as PDF.
  
## Screenshots

![Screenshot 2025-02-08 143143](https://github.com/user-attachments/assets/71ebfe5f-4f38-4847-82b2-63134a63f036)
![Screenshot 2025-02-08 143222](https://github.com/user-attachments/assets/bb8ca304-839c-4f06-9a13-e03eff868e39)
![output-pdf-file](https://github.com/user-attachments/assets/ef1bba24-93de-4e4e-83bc-3967a583392b)

## Dependencies

This project leverages several popular libraries hosted via CDNs:
- **[Marked](https://cdn.jsdelivr.net/npm/marked/marked.min.js):** For Markdown parsing.
- **[Highlight.js](https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.5.0/highlight.min.js):** For code syntax highlighting.
- **[Chart.js](https://cdn.jsdelivr.net/npm/chart.js):** For rendering the messages per month chart.

## Notes

- **How to Export Chats in WhatsApp as a .txt File?**
  Open the conversation you wish to print. Click on 3 dots > More > Export Chat > Without Media and use [On Device](https://github.com/lmj0011/save-on-device) to save to to your phone's storage. Alternatively, you can also mail it to yourself to use this converter on your PC. 

- **Client-Side Only:**  
  All processing occurs in your browser. No data is sent to any server. 

- **Transcript Format:**  
  The parser expects a format similar to:

  12/31/20, 11:59 PM - John Doe: Happy New Year!

  Additional lines that do not match the initial pattern are appended to the previous message.

## License

This project is open source and available under the Apache License 2.0. 

## Acknowledgments

- Thanks to the developers of [Marked](https://github.com/markedjs/marked), [Highlight.js](https://highlightjs.org/), and [Chart.js](https://www.chartjs.org/) for providing these fantastic libraries. This project was entirely created with [DeepSeekR1](https://github.com/deepseek-ai/DeepSeek-R1) and o3-mini. 

