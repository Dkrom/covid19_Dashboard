# Covid19_Dashboard

Analyse our country's Covid19 situation using python.

# Screenshots

![covid cases](https://user-images.githubusercontent.com/86722467/180482952-9f811e11-3610-40ad-abbd-a8670dc4d0ec.png)

![covid deaths](https://user-images.githubusercontent.com/86722467/180483102-af9fc64c-eb87-4630-a055-ad91bd6e0e21.png)

![positivity](https://user-images.githubusercontent.com/86722467/180483223-cdacb8e7-6160-42aa-9c20-02b903ae8449.png)

# Installation

Install required modules using:

```
pip install pandas
pip install numpy
pip install matplotlib
```
# Usage/Examples

Read the data from CSV file:

```
df=pd.read_csv("https://raw.githubusercontent.com/owid/covid-19-data/master/public/data/owid-covid-data.csv")
```

Convert string Date time into Python Date time object.

```
df['date']=pd.to_datetime(df['date'], errors='coerce')
```
Visualize covid19 cases in india:
```
plt.plot(india_cov19.date, india_cov19.new_cases)
plt.xlabel('Date')
plt.ylabel('New cases')
plt.title("Covid-19 New cases in India")
plt.show()
```
