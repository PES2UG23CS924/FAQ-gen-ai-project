# Automated FAQ Bot

**Customer Support Bot using Transformer-Based Question Answering**

---

## Project Overview

This project implements an **Automated FAQ Bot** that answers user questions based on a company’s policy document. Instead of manually searching through long policy texts, users can ask questions in natural language and receive accurate answers extracted directly from the document using a transformer-based Question Answering model.

---

## Objective

* To automate FAQ responses for customer support
* To demonstrate **extractive Question Answering** using transformers
* To apply Hugging Face NLP pipelines covered in **Unit 1**

---

## Technology Used

* **Programming Language:** Python
* **Library:** Hugging Face `transformers`
* **Pipeline:** `question-answering`
* **Model:** `distilbert-base-cased-distilled-squad`
* **Input Document:** Text file (`.txt`)

---

## Project Structure

```
PES2UG23CS924/
│── FAQbot.ipynb
│── SampleCompanyPolicy.txt
│── PES2UG23CS924_Observation_faq.pdf
│── README.md
```

---

## How It Works

1. The company policy document is stored in `SampleCompanyPolicy.txt`.
2. The document is loaded as **context** for the Question Answering model.
3. The user enters a question through an interactive input.
4. The transformer model extracts the most relevant answer span from the document.
5. The system displays the answer along with a confidence score.

---

## How to Run the Project

1. Install required libraries:

   ```bash
   pip install transformers torch
   ```

2. Make sure `SampleCompanyPolicy.txt` is in the same folder as `FAQbot.ipynb`.

3. Open and run `FAQbot.ipynb`.

4. Ask questions such as:

   * Who should salary discrepancies be reported to?
   * What are the customer support hours?
   * How many days of paid leave are employees entitled to?

5. Type `exit` to stop the bot.

---

## Sample Output

```
Question: Who should salary discrepancies be reported to?
Answer: HR
Confidence Score: 1.64
```

---

## Observations

* The bot provides accurate answers when the information is clearly present in the policy document.
* Well-phrased and specific questions result in higher confidence scores.
* The system avoids hallucination by extracting answers directly from the given text.
* The model performs efficiently on CPU without requiring fine-tuning.

---

## Limitations

* The bot cannot answer questions whose answers are not present in the document.
* Ambiguous or informal questions may reduce accuracy.
* Designed for single-document Question Answering only.

---

## Conclusion

The Automated FAQ Bot demonstrates an effective use of transformer-based extractive Question Answering for customer support applications. By leveraging a pretrained DistilBERT model, the system provides reliable and efficient access to information stored in company policy documents.

---

## Author

* **Name:** *KRITHIKA A*
* **SRN:** *PES2UG23CS924*
* **Course / Section:** *E*

