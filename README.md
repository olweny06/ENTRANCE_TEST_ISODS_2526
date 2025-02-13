# Phap Dien Document Crawling and Search Project

## Description

This project consists of three Python notebooks designed to crawl and process data from the Phap Dien website (phapdien.moj.gov.vn).
The objectives of the project are:

1. **Crawling the Phap Dien Website**:

   - Download the Phap Dien document from the provided link: [Download Phap Dien](https://phapdien.moj.gov.vn/TraCuuPhapDien/Files/BoPhapDienDienTu.zip).
   - Unzip the downloaded file and create additional directories: `vbpl`, `property`, `history`, `related`, and `pdf` under the `BoPhapDienDienTu` directory.
   - Iterate through each index HTML file in the `demuc` directory and save the linked HTML documents in the appropriate directories with specific naming conventions.

2. **Creating a Vector Database**:

   - Use ChromaDB (via LangChain) to create a vector database that ingests only the document files (full_ItemID.html).
   - Ensure that the file path is saved in the metadata.

3. **Performing Semantic Search**:
   - Implement a semantic search on the vector database using LangChain and return the top k results.
   - Comment on the observations from the search results.

## Requirements

- Use the following embedding model that supports Vietnamese: [Vietnamese Bi-Encoder](https://huggingface.co/bkai-foundation-models/vietnamese-bi-encoder) (chunk size = 2000 tokens, chunk overlap = 20 tokens).
- Code is preferably written in a Colab notebook.
- Add sufficient comments and docstrings in your code.
- Submission is in the form of a GitHub repository to be sent back via email. A README file is required.
- Code should be in the repository. Large data files and vector databases should be shared separately via Google Drive.

## Usage

- Code in Google Colab, Jupyter Notebook
- Follow the instructions in each notebook to execute the crawling, database creation, and search functionalities.
- Ensure that you have the necessary libraries installed, such as `requests`, `beautifulsoup4`, `langchain`, and `chromadb`.

## Data Files and Vector Databases

The following links provide access to the large data files and vector databases used in this project:

- [Download BoPhapDienDienTu Data] https://drive.google.com/drive/folders/1kGEwy2yhP_doNGvUasd2KbpoM-bqTLDb?usp=drive_link
- [Download Vector Database] https://drive.google.com/drive/folders/1BXcP5ytmeiHDEC4bKkqtZxqCaRgOwjs1?usp=drive_link

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
