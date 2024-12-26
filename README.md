# OCR

## Objective  
To extract useful entities from different Invoice Images:  
1. **Invoice Number**  
2. **Invoice Date**  
3. **Customer Name**  
4. **Total Amount in Invoice**  

## Challenges with Vanilla OCR  
Vanilla OCR extracts text line by line from Invoice Images, but there’s no fixed format in such documents. Hence:  
- **Regex-based approaches** or **Python string matching** methods do not work effectively.  

## Explored Techniques  
1. **Extract OCR, clean text, and use LLM with prompts**  
   - Extract the OCR text.  
   - Clean and preprocess the text.  
   - Pass the cleaned text to an LLM with a specific prompt to extract the required entities.  

2. **Pretrained models for Document Question Answering**  
   - These models are trained on a large corpus of Invoices, Receipts, and Documents to understand layouts and extract relevant entities.

3. **Vision-Language Models (VLM) with prompting**  
   - Use VLMs with appropriate prompting techniques to extract useful entities directly from the images.  

## Conclusion  
Among all the explored techniques, **Vision-Language Models (VLM)** provided the best performance.
