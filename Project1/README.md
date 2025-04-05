## Salary-Dashboard

 excel skills used:
 _ ❎data validation
 _ 🧮formulas and functions
 _ 📉Charts

 ## main formula 
This is the primary formula used to calculate the median salary, allowing us to perform  analysis based on its results.
 ```
 =MEDIAN(
  IF(
    (jobs[job_title_short]=$A4)*
    (jobs[salary_year_avg]<>0)*
     (jobs[job_country]=country)*
     (ISNUMBER(SEARCH(type,jobs[job_schedule_type]))),
    jobs[salary_year_avg]
  )
)

 ```
  
