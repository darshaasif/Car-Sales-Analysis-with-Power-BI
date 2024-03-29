# Car-Sales-Analysis-with-Power-BI
Formulas I used
Calender = CALENDAR(DATE(starting date),DATE(end date ))
current year = 2023
Month = FORMAT([DATE],"MMM")
month_index = MONTH([DATE])
month year = FORMAT([DATE],"MMM")&"-"&RIGHT([year],2)
pre year = [current year]-1
YEAR = YEAR([DATE])
Growth = DIVIDE([yttcurrent_sales],[yttprev_sales])
sale = SUM(Details_1[Value])
yttcurrent_sales = var currentyear=[current year]
   return CALCULATE([ytdsales],'Calender'[YEAR]=currentyear)
YTD SALES
YTD_SALES=totatytd(sum(tablename[sales])),’calender’[date])
Or
ytd_sales=calculate([sales],datesytd(‘calender’[date])
Prev year sales = calculate ([sales],sameperiodlastyear(‘calender’[date]))
   
