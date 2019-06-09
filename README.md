# Vietnam-War-Info-Wiki
<h1> Report</h1>


Below is an image of a Power BI Dashboard that I created(File - Vietnam.pbix). The data was obtained from Wikipedia using web scrapping. The concept behind the Dashboard was to create a document that would be able to able to give an overview of each battle that occurred during the Vietnam War. This includes :

<ul> 
  <li>The location of the Battle</li>
  <li>A Searchable Timeline </li>
  <li>A Breakdown of Regional and City Battles</li>
  <li>An Account of the Causalities for each Battle </li>
  <li> A Description of each Battle.</li>
  <li> The exact Time of each Battle. </li>
</ul>

Figure 1 - Final Dashboard 
<img src="Vietnam.JPG">
  
<h1> Getting the Data and Cleaning it up </h1>

The full code that was created to collect and clean the data can be found in the file "Python_code.ipynb". Below I will quickly explain the steps that I took to get the data. 

<h2> Step 1 - Webscrapping the Data</h2>
I used Pandas and its read_html tool to upload the data from Wikipedia into a Pandas dataframe.

Figure2 - Webscrapping Code
<img src="wiki_data.JPG">

However, this produced a table that contained data that would be very difficult to use as there was no consistant date or location format.

Figure 3 - Original Dataframe
<img src="wiki_original_data.JPG">

<h2> Step 2- Cleaning up the Data </h2> 

I then used a number of  regular expression and normalization techniques to :

<ul>
  <li>Reformat the Data</li>
  <li>Split the Location into Province and Cities </li>
 </ul>
 
 Figure4 - Regular Expressions
 <img src="reg_expressions.JPG">
 
<h2> Step 3 - Use Power BI to Create Dashboard</h2>

Once the data was in a better format, I uploaded the data into the Power BI desktop and used the software's tools to create the dashboard from figure 1. 
