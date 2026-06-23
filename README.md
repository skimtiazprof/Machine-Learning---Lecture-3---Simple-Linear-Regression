# Machine-Learning---Lecture-3---Simple-Linear-Regression
A Simple Linear Regression project built with Python, Pandas, Matplotlib, and Scikit-learn to predict house prices based on house size. This project covers data preprocessing, model training, prediction, and professional data visualization with a regression line, customized plots, and annotations for better understanding.
plt.figure(figsize=(12,7))

plt.xlabel("House Size (sqft)", color="blue", fontsize=18)
plt.ylabel("Price (USD)", color="green", fontsize=18)

plt.scatter(df.House_Size_sqft, df.Price_USD,
            color="green", s=15, label="Actual Data")

plt.plot(df.House_Size_sqft,
         lr.predict(df[["House_Size_sqft"]]),
         color="red",
         linewidth=2,
         label="Regression Line")

plt.title("House Size vs Price Prediction",
          fontsize=22,
          color="purple",
          fontweight="bold")

plt.legend(fontsize=12)

plt.text(1200, 430000,
         "Learn AI/ML",
         fontsize=50,
         color="gray",
         alpha=0.20,
         rotation=25)

plt.text(2800, 300000,
         "By Zafar Iqbal",
         fontsize=15,
         color="red",
         alpha=0.7,
         fontstyle="italic")

plt.grid(alpha=0.3)
plt.show()
