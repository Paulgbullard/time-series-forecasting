# Time Series Forecasting with R and Prophet

This Shiny app was originally developed to work alongside the NHS England and NHS Improvement Demand and Capacity Team's Urgent and Emergency Care models. It uses Prophet to automate time series forecasting for type 1, 2 and 3 emergency departments.

# Use

The app can be used with any hourly time series data to forecast forward for 168 periods, or one week. The resulting output is the expected value (hourly) with 85% confidence intervals.

More than one variable can be predicted. If this is the case, models are created for each variable individually. 

# Locked Parameters

The app uses the following flags within Prophet:

```r
yearly.seasonality = TRUE
monthly.seasonality = TRUE
daily.seasonality = TRUE
interval.width = 0.85
add_country_holidays('England')
```

These are not editable by the user.
