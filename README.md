# 🔍 Declassified JFK Files Summary

## 📜 Overview
This repository contains AI-generated summaries of declassified JFK assassination files. With over 1,000 original documents, this project makes these historical records more accessible and digestible.

![Government agent examining files](/images/glowie.jpg)

The documents explore the investigation of **Lee Harvey Oswald** and his connection to President Kennedy's assassination. They come from CIA and intelligence files released under the **JFK Assassination Records Act**.

### TODO
- Add more details about the content of the files
- Include the Go code used to process the files (work in progress to improve a bit)

### Tldr;
- **Oswald's movements and contacts** – His trip to Helsinki and interactions with Soviet officials.  
- **Government coordination** – How the CIA and State Department handled Oswald's return from the Soviet Union.  
- **Official investigations** – Reports and discussions from the **Warren Commission** and the **House Select Committee on Assassinations (HSCA)**.  
- **Oswald in Mexico City** – A detailed timeline of his visits to the Cuban and Soviet embassies.  
- **KGB assessment** – Testimony from Soviet defector **Yuri Nosenko**, stating that the KGB considered Oswald "uninteresting."  
- **Cuban involvement?** – A task force investigated possible links to Fidel Castro's regime but found no solid evidence.  
- **Conspiracy theories** – Speculation that an "unidentified man" photographed in Mexico City was a Soviet agent, **Yuriy Ivanovich MOSKALEV**.  
- **FBI reports** – Internal memos mentioning potential Cuban connections to the assassination.  

While **Oswald is a key figure in these investigations**, the documents do not provide a clear answer on who killed President Kennedy.
Instead, they focus on various leads, intelligence reports, and Oswald's actions before and after the assassination.

## 🤖 AI Models Used
- **OpenAI** - Using o3-mini by default, summaries in `openai-o3-mini/`
- **Gemini** - Summaries in `Gemini-flash/`

## 🔧 Technical Process
- Documents were processed in batches using **Golang**
- Batch sizes of 15, 20 and 25 documents were used for efficient processing
- Different batching sizes were used to test the performance of the AI models
- API rate limits and timeouts were handled with retry mechanisms
- All summaries are preserved in Markdown format

## 📊 Repository Structure
- `Gemini-flash/batches-of-15/` - 68 batch summary files from Gemini
- `Gemini-flash/batches-of-20/` - 51 batch summary files from Gemini
- `openai-o3-mini/batches-of-25` - 41 batch summary files from OpenAI
- `openai-o3-mini/batches-of-15` - 68 combined summary files from OpenAI

## Audio
- Summary of the JFK files in audio format as a podcast episode can be found in the `audio/podcast` folder

## 🧠 Why AI Summaries?
The original declassified JFK files contain thousands of pages of complex information. These AI-generated summaries help researchers and history enthusiasts navigate this vast collection more efficiently.

## 📚 Reading the Summaries
Each summary file maintains references to original document IDs and preserves important details like names, dates, and key facts while condensing the information into readable formats.

---

## Credits & Original link to JFK Files
The Declassified JFK Files released by the CIA can be found [here](https://www.archives.gov/research/jfk/release-2025)
Original markdown conversion of the JFK files by [Amjad Masad](https://github.com/amasad/jfk_files/tree/main)