🛍️ Fashion Trend & Sales Forecasting App
This project combines data analytics, image processing, and social sentiment analysis to forecast fashion product sales, visualize public opinion, and showcase trending fashion items. Built using Python, PRAW (Reddit API), Unsplash API, and Gradio UI, it leverages real-time trends and seasonal insights to assist fashion retailers and enthusiasts in informed decision-making.

🚀 Features
📊 Sales Forecasting using SARIMAX time series model

🖼️ Fashion Image Recommendation powered by ResNet50

💬 Sentiment Analysis from Reddit comments using TextBlob

📈 Fashion Trends Detection using curated monthly trend data

📅 Festival Awareness for seasonal sales planning

🧠 Visual Comparison of trending vs selected product images

🌐 Interactive Web Interface using Gradio

📂 Dataset
Fashion_Retail_Sales_Modified.csv
Contains data on:

Country

Date of Purchase

Product Type

Purchase Amount (USD)

🔧 Tech Stack
Frontend/UI: Gradio

Backend/Data: Python, Pandas, StatsModels

ML/AI Models: ResNet50 (TorchVision), SARIMAX

APIs: Reddit API (via PRAW), Unsplash API

Visualization: Matplotlib

Others: TextBlob (sentiment analysis), PIL, NumPy

📸 Image Handling
Retrieves images from Unsplash for given fashion products

Selects the most representative image using feature extraction from ResNet50

Stores images locally in the /fashion_images/ directory

📥 Installation
bash
Copy
Edit
git clone https://github.com/yourusername/fashion-trend-sales-app.git
cd fashion-trend-sales-app
pip install -r requirements.txt
Make sure to create a .env file or directly input your API keys in the script for:

Reddit API

Unsplash API

▶️ Run the App
bash
Copy
Edit
python app.py
The app will launch in your browser via Gradio with a public shareable link.

🌐 APIs Used
Reddit API: Fetches fashion discussions & comments

Unsplash API: Downloads high-resolution fashion product images

📈 Forecasting Logic
Uses SARIMAX (Seasonal ARIMA) model to forecast future sales:

Grouped by Month

Forecast up to 3 years

Predicts revenue based on expected units sold and market trend

🔍 Example Use Case
Select a country and product

Enter a future sale date (e.g., 2025-12) and expected units

Get:

Predicted revenue

Sentiment analysis pie chart

Trending fashion items with image previews

Festival and seasonal insights

📂 File Structure
bash
Copy
Edit
fashion-trend-sales-app/
│
├── fashion_trends.py             # Contains monthly trend keywords
├── app.py                        # Main Gradio app and all backend logic
├── Fashion_Retail_Sales_Modified.csv
├── fashion_images/               # Folder for downloaded images
├── sentiment_pie_chart.png       # Auto-generated sentiment chart
└── README.md
📌 Todo / Improvements
 Add user authentication

 Use deep learning for better sentiment classification

 Real-time news scraping for trending updates

 Integrate Instagram/Facebook trend APIs

🙌 Acknowledgements
Reddit for user sentiment data

Unsplash for fashion images

TorchVision and ResNet for image feature extraction

Gradio for seamless app interface

📬 Feedback
If you have any suggestions or improvements, feel free to submit a PR or raise an issue.
💬 Let us know your thoughts via the feedback box in the app!

📃 License
MIT License

