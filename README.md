# sentiment_analysis_dart

The original code defines a TextAnalyzer class with a single static method, isTextAppropriate, which does the following:

Configuration:
It retrieves an API key from environment variables using the flutter_dotenv package.

API Request:
It builds a POST request to a text analysis API endpoint (in this case, Google's Natural Language API) by including the API key in the URL and sending a JSON payload containing the text to analyze.

Sentiment Analysis:
The API returns a sentiment score (typically between –1 and 1). The method then checks if the sentiment score is below a threshold (less than –0.5 in this example). If it is, the text is deemed inappropriate; otherwise, it’s considered acceptable.

Error Handling:
If the API call fails, the error is printed and the function returns false.
