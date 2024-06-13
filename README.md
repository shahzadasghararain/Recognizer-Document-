This repository contains a Python script designed to analyze documents using Azure's Form Recognizer service. The script extracts textual content, layout information, and identifies handwritten content within the document. Key features include:

1. **Azure Form Recognizer Setup:**
   - Utilizes `azure.core.credentials` and `azure.ai.formrecognizer` for accessing Azure Cognitive Services.
   - Configures the endpoint and API key for authentication.

2. **Bounding Box Formatting:**
   - Includes a helper function `format_bounding_box` to format bounding box coordinates for better readability.

3. **Document Analysis:**
   - Defines the `analyze_read` function to analyze a sample document from a specified URL.
   - Initializes the `DocumentAnalysisClient` with the configured endpoint and credentials.
   - Submits the document for analysis and retrieves the results.
   - Prints the document content and identifies the presence of handwritten content.
   - Iterates through the pages, lines, and words in the document, printing text content, bounding boxes, and confidence scores.

4. **Main Execution:**
   - Calls the `analyze_read` function if the script is executed as the main module.

To set up and run the script:
- Ensure you have the necessary dependencies installed (`azure-core` and `azure-ai-formrecognizer`).
- Replace the placeholder endpoint and key with your actual Azure Cognitive Services endpoint and API key.
- Run the script to analyze the sample document and view the extracted content and layout information.

This script provides a straightforward way to leverage Azure's Form Recognizer service for document analysis and extraction of structured information.

