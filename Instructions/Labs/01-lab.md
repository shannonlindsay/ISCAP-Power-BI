---
lab:
    title: 'Lab Instructions'
    module: 'Hands on Lab'
---

# Build your first Power BI report

This lab is designed to introduce you to the Power BI Desktop application, and enable you to practice basic data transformation and build data visualizations. This lab only introduces the concept of building reports using Power BI desktop. It does NOT go into publishing and sharing reports, scheduling automated refreshes, or anything using the Power BI service.

## Dataset

This exercise uses maximum ice coverage data from NOAA’s Great Lakes Environmental Research Laboratory. A lake can have ice coverage ranging from 0 (no ice) to 100 (frozen over).

**[Download the data](https://4lbi-my.sharepoint.com/:x:/p/shannon/EYE_uUd1hENBqjx5v_yGAuABcSmFG6IUj14_j0EfJUnKTQ?e=O4jpeI)** prior to starting the exercise. **Save the dataset** in a location you'll remember.

**This lab should take approximately 45 minutes.**

Working together we will get started, get and transform data, and build your first visual. You'll then have time to play around with the data, add additional visuals to your page and add your own design flair!

## **Get and Transform Data**

1. Open a Power BI Desktop file.

1. Save a copy of the file using **Save As** - name the file and save to a place you'll remember.

1. On the **Home** ribbon tab, from inside the **Data** group, select **Excel**. Step through the wizard, select **Sheet 1**, and select **Transform Data**.

   *This will open the Power Query editor window. This is where we'll transform our data for analysis.*

1. From here, we need to shape our data so that we can easily look at our data by year and by lake. We want to end up with a single column for lakes. You will use the **Unpivot Other Columns** option on the transform tab of the ribbon to achieve this.
   
3. Using the options in the tranform tab of the ribbon, fix the formatting of the lake names so they are all capitalized.

   *Take a look at all of the options on the transform tab of the ribbon. Let me know if any of these raise questions!*

1. Rename the Attribute and Values column to something that makes sense to you.

   *That's it - our data is transformed and in shape to start building visualizations!*

1. On the Home tab of the Ribbon, select **Close and Apply**. This applies the changes you made to the data to the **[Data Model](https://www.phdata.io/blog/data-modeling-fundamentals-in-power-bi/)**. 

## Build a Matrix Visual

The blank canvas in Power BI can be intimidating! There are a million buttons and panes - lets take a moment to explore together before jumping in.

I always like to start with a table visual to understand what my data looks like. After we get our table on the canvas, we'll add a slicer visual together and explore conditional formatting.

1. From the insert tab of the ribbon, select the **Matrix** visual. This will drop a blank table on the canvas.
   
1. Use the **Add data** button in the **Build a visual** pane to add columns from your data to the table.

2. When you add the **Year** column to the table, it will automatically sum. To avoid columns summing that should not, select the column in the **Data** pane, and change the summarization on the **Column tools** tab of the ribbon to **Don't summarize**.

3. Play around with adding fields to the rows, columns, and values field wells in the **Build a visual** pane. Understanding where your data will go when you populate these fields is key to your success!
4. Turn the totals off for the visual using the **Format** pane (looks like a tiny paintbrush on the right-hand side of the screen).
5. Apply any other customizations you'd like to the formatting of your matrix visual. Ask questions as needed.

## Add a slicer visual to enable users to select a range of years

1. Add a slicer visual using the **Insert** tab of the ribbon.

2. Customize the appearance of your slicer using the **format pane** and change the name to make it user friendly.
   
4. Play around with the slider to see how it works!

## Add a line chart displaying the average ice coverage over time

1. Add a line chart using the insert tab of the ribbon
2. Power BI will automatically **Sum** the ice coverage value field. Select the column name in the **Build a visual** pane and change the aggregation from sum to **average**.
    
    *Power BI is smart and can automatically create calculations for you. These calculations are called **measures**. When a measure is automatically created in a visual, this is called an **implicit measure**.*

1. Let's practice writing our first explicit measure using the DAX language. We'll create a measure for, you guessed it, the average ice coverage. This is a different way of accomplishing the same thing, but, can also be used elsewhere in other visuals.
   *Read more about implicit vs explicit measures on [Reza's blog](https://radacad.com/explicit-vs-implicit-dax-measures-in-power-bi)*

1. Add your new **average ice coverage** measure to your line chart visual.

2. Format your line chart. Add and remove labels, gridlines, axis labels - whatever you prefer the formatting to look like.
   *Pro tip: use the search bar at the top of the formatting pane!*

1. Add a **trend line** to see what's going on with average ice coverage over time. Find this on the **Format** pane.

## Add a column chart displaying the maximum ice coverage by lake

1. Using similar methods as above, add a column chart to your canvas and include the fields **Lake** and **Ice coverage**. This time we want to look at **Maximum ice coverage** - use the UI to create your measure or write a new explicit measure using DAX.
2. Format your bar chart using the **Format** pane.

## Format your report

1. Add a title and data source to your report.
2. Move the visuals around so that they make sense to both your eye and how you want to display the data. 

## Moving fast?! Play around with different types of visuals!

<img width="1581" alt="image" src="https://github.com/shannonlindsay/ISCAP-Power-BI/assets/77289548/6eabd5a7-1b7f-44ef-869c-149c26f0a109">


## Check your work

You can [download a copy](https://4lbi-my.sharepoint.com/:u:/p/shannon/EQR0NN474plHtOlVfnowNqYBflQrm6OHabqzHtvLAfs81Q?e=ZRb7p2) of the completed report to see what I've done.

 
