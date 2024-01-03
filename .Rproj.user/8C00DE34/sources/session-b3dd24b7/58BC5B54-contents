data("mtcars")
mtcars

Data_Cars <- mtcars
dim(Data_Cars)

names(Data_Cars)
rownames(Data_Cars)
Data_Cars <- mtcars
Data_Cars$cyl

Data_Cars <- mtcars
sort(Data_Cars$cyl)

max(Data_Cars$hp)
min(Data_Cars$hp)

Data_Cars<-mtcars
summary(Data_Cars)

Data_Cars <- mtcars
mean(Data_Cars$wt)

Data_Cars <- mtcars
median(Data_Cars$wt)

Data_Cars <- mtcars
names(sort(-table(Data_Cars$wt)))[1]

Data_Cars <- mtcars
quantile(Data_Cars$wt, c(0.75))



library(forecast)


sales_data <- data.frame(
  Month = seq(as.Date("2023-01-01"), as.Date("2023-06-01"), by =
                "months"),
  Sales = c(12000, 15000, 18000, 16000, 20000, 22000)
)



sales_ts <- ts(sales_data$Sales, frequency = 12,start=c(2023,1))
print(sales_ts)

arima_model <- auto.arima(sales_ts)

# Forecast sales for next 3 months
forecast_result <- forecast(arima_model, h = 3)

# Display forecast results
print(forecast_result)

plot(forecast_result)
