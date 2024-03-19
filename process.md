# Process

1. Export timeline data from the Libby app in CSV format.
2. Clean and import the date to Excel using Power Query. Do initial cleaning in Excel.
3. Determine questions to ask of the data:
   1. Which library did I borrow from most frequently?
      1. overall
      2. by year
      3. by quarter
      4. by month
   2. Were there some books I placed on hold but didn't check out?
   3. How many books did I borrow?
      1. overall
      2. by year
      3. by month
   4. Which books did I renew?
   5. When (what dates) did I borrow books?
      1. Are there periods when I borrowed more than the norm?
      2. Are there periods when I borrowed less than the norm?
   6. Are there patterns in the time of day that I checked books out?
   7. Explore data in Tableau in an effort to answer these questions.
      1. Notice that I needed to make a calculated field in Tableau called "Author1.full," because I have at least two authors with the same family name.
      2. Decide to ignore any authors other than the first, since the first author is sufficient to tell me what I really want to know about whom I'm reading.
      3. Notice that Indiana Digital Library and Indiana Digital Download Center are both listed. These are actually the same library. Create a new calculated field in Tableau to change "Indiana Digital Download Center" to "Indiana Digital Library." That way my visualizations will correctly show four libraries in the data set, rather than five.
      4. Create a variety of visualizations to explore the data.