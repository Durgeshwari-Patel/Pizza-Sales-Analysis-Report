# 🍕 Pizza Sales Analysis Dashboard (Power BI)

An interactive, two-page Power BI report that analyzes a full year (Jan–Dec 2015) of pizza sales. It tracks the main business KPIs, shows when and what customers order, and ranks the best and worst selling pizzas.

---

## 📌 Project Overview

A pizza business needs to know how it is performing over the year, which products drive sales, and when customers order the most. This dashboard answers those questions in one place and lets users filter the data by date range and pizza category.

### Business questions answered
- How much revenue, how many orders, and how many pizzas were sold in the year?
- What is the average order value and the average number of pizzas per order?
- How do orders change by month and by day of the week?
- Which pizza categories and sizes contribute the most to sales?
- Which pizzas are the best sellers and which are the worst, by revenue, quantity, and number of orders?

---

## 📊 Dashboard Pages

### 1. Home – Sales Performance
<img width="1342" height="748" alt="home" src="https://github.com/user-attachments/assets/3700a081-493c-4315-9701-cd0e58ec34bb" />







| Visual | What it shows |
|---|---|
| KPI cards | Total Revenue, Total Orders, Total Pizzas Sold, Average Order Value, Average Pizzas per Order |
| Area chart | Monthly trend of total orders |
| Column chart | Total orders by day of the week |
| Donut chart | % of sales by pizza category |
| Donut chart | % of sales by pizza size |
| Funnel chart | Total pizzas sold by pizza category |
| Slicers | Order date range and pizza category |

### 2. Best / Worst Sellers
| Visual | What it shows |
|---|---|
| Top 5 / Bottom 5 bar charts | Pizzas ranked by **Total Revenue** |
| Top 5 / Bottom 5 bar charts | Pizzas ranked by **Total Pizzas Sold** (quantity) |
| Top 5 / Bottom 5 bar charts | Pizzas ranked by **Total Orders** |
| KPI cards | The same five KPIs, responding to the filters |
| Slicers | Order date range and pizza category |

Both pages have page-navigation buttons so users can move between them.

---

## 🖼️ Dashboard Preview

### Home – Sales Performance
![Home page](images/home.png)

### Best / Worst Sellers
![Best and Worst Sellers page](images/best_worst_sellers.png)

---

## 🔍 Key Insights

**Overall (Jan–Dec 2015):** 817.86K total revenue, about 21K orders, about 50K pizzas sold, an average order value of 38.31, and 2.32 pizzas per order.

- **Days:** Friday is the busiest day (3.5K orders), followed by Thursday and Saturday (3.2K each). Sunday is the slowest day (2.6K).
- **Months:** July has the most orders (1,935). Orders are also high in January, March, May, and August (about 1,840–1,853) and lowest in September and October (1,661 and 1,646).
- **Category:** Classic is the top category with 26.91% of sales and 14,888 pizzas sold. Supreme follows with 25.46%, then Chicken (23.96%) and Veggie (23.68%).
- **Size:** Large pizzas bring in the most sales at 45.89%, followed by Medium (30.49%) and Regular (21.77%). X-Large and XX-Large together are under 2%.
- **Best sellers:** The Thai Chicken pizza earns the most revenue (43K), while The Classic Deluxe pizza leads in both quantity sold (2.5K) and total orders (2.3K).
- **Worst seller:** The Brie Carre pizza is the lowest on all three measures: 11.6K revenue, 490 pizzas sold, and 480 orders.

---

## 🗂️ Data Model

The report uses one table, `pizza_sales`, with these fields:

| Field | Description |
|---|---|
| `order_date` | Date of the order |
| `Order Month` | Month derived from the order date |
| `Order Day` | Day of the week derived from the order date |
| `pizza_name` | Name of the pizza |
| `pizza_category` | Category of the pizza (for example Classic) |
| `pizza_size` | Size of the pizza (for example Large) |

### DAX measures
| Measure | Meaning |
|---|---|
| `Total Revenue` | Total sales amount |
| `Total Orders` | Number of orders |
| `Total Pizzas Sold` | Total quantity of pizzas sold |
| `Avg Order Value` | Average revenue per order |
| `Avg Pizza Per Order` | Average number of pizzas per order |

---

## 🛠️ Tools & Skills Used

- **Power BI Desktop**
- **DAX** for calculated measures and columns
- **Data modeling and cleaning** in Power Query
- **Data visualization:** KPI cards, area, column, donut, funnel, and bar charts
- **Report design:** slicers, Top N filters, page navigation, and a consistent layout with custom icons

---

## 🚀 How to Use

1. Download or clone this repository.
2. Open `Pizza_Project.pbix` in **Power BI Desktop** (free to download from Microsoft).
3. Use the date and category slicers to explore the data.
4. Use the navigation buttons to switch between **Home** and **Best/Worst Sellers**.

---

## 📁 Repository Structure

```
├── Pizza_Project.pbix      # Power BI report file
├── images/                 # Dashboard screenshots
│   ├── home.png
│   └── best_worst_sellers.png
└── README.md
```

---

## 👩‍💻 Author

**Durgeshwari Patel**
Aspiring Data Analyst | SQL · Power BI · Python

- 📧 durgeshwaripatel1811@gmail.com
- 🔗 [LinkedIn](https://linkedin.com/in/durgeshwari-patel-18112771pp)
