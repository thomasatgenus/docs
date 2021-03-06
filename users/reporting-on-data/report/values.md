## Values

A value is bound to an object, for example the sales amount for an employee. A value defines numerical data in the report when it is placed in the **Values** field.

You can find the values in the object folders they belong to. To place data sources and values in the report, you can use a drag-and-drop operation. To change the settings for the value, right-click on the value and perform appropriate settings.

![IDDE03783BDCB147B9.ID0C0ECD20B7B94C1D.png](media/IDDE03783BDCB147B9.ID0C0ECD20B7B94C1D.png)

<table style="WIDTH: 100%">

<tbody>

<tr>

<th>Value Options</th>

<th>Description</th>

</tr>

<tr>

<td>**Open**</td>

<td>Open the value properties. In the **General** tab you can set the name, number format for the values. The **Connections** tab contains a list over the valueb s connections to objects.</td>

</tr>

<tr>

<td>**Copy**</td>

<td>Copy a value</td>

</tr>

<tr>

<td>**Paste**</td>

<td>Paste the copied value into the values field.</td>

</tr>

<tr>

<td>**Insert**</td>

<td>Insert Formula, Function, or If condition into to values field.</td>

</tr>

<tr>

<td>

**Format**

</td>

<td>

Customize number and chart.

*   **Number** set the number format on the value.
*   **Chart** <span style="FONT-WEIGHT: normal">s<span style="FONT-WEIGHT: normal">et the valueb s appearance in charts. You can set the appearance, value axis, lines and points for chart.

</td>

</tr>

<tr>

<td>

**Rename**

</td>

<td>

Rename the value. This will also affect the column name in the report if the value is shown as a column.

</td>

</tr>

<tr>

<td>**Connections**</td>

<td>Set which objects in the report the value relates to.</td>

</tr>

<tr>

<td>

![IDDE03783BDCB147B9.ID83D2DB038AA44C15.jpg](media/IDDE03783BDCB147B9.ID83D2DB038AA44C15.jpg)**Local Filters**

</td>

<td>

Set filter direct on the value for the data sources which is placed in Filters field. Local filters in value will overrule the filter in the report.

*   **None** <span style="FONT-WEIGHT: normal">n<span style="FONT-WEIGHT: normal">one members selected.
*   ****Selection** <span style="FONT-WEIGHT: normal">manual selected members.**
*   ****Criteria** <span style="FONT-WEIGHT: normal">members from search result by given criteria.**
*   **[Saved data Filter**](../../../developers/defining-the-application-model/data-filters.md) <span style="FONT-WEIGHT: normal">insert predefined data filter as filter

</td>

</tr>

<tr>

<td>

**Local Aggregation**

</td>

<td>

Aggregate the value based on selected object.

</td>

</tr>

<tr>

<td>![IDDE03783BDCB147B9.IDD572BD670A164A4B.jpg](media/IDDE03783BDCB147B9.IDD572BD670A164A4B.jpg)  **Series Calculation**</td>

<td>Calculate the value based on the object or code in horizontal axis or vertical axis. A Series Calculation can for example be a sum, average, median, max, min and so on.</td>

</tr>

<tr>

<td>![IDDE03783BDCB147B9.ID1DAC325DF02445D6.jpg](media/IDDE03783BDCB147B9.ID1DAC325DF02445D6.jpg)  **Rank and Cut**</td>

<td>

Sort and cut data in table on the value you are trying to rank. Example the function is useful when you want to show only the bottom 10 or bottom 10 results in a table. This function is only available when no objects are placed in horizontal axis and there is only one object placed in vertical axis.

</td>

</tr>

<tr>

<td>![IDDE03783BDCB147B9.IDCED84F1921EE47BD.jpg](media/IDDE03783BDCB147B9.IDCED84F1921EE47BD.jpg)  **Period Shift**</td>

<td>

Shift time period on the value according to Time Reference. This function makes it easy to compare values in different time period.

To add Period Shift on a value, the time will shift back or forward in time.

<span style="FONT-WEIGHT: bold; FONT-STYLE: italic">Name set the name for the value  
<span style="FONT-WEIGHT: bold; FONT-STYLE: italic">Shift set the number of time period which shall move back or forward according to time reference in the filter.  
<span style="FONT-WEIGHT: bold; FONT-STYLE: italic">Type set the type of time period.

![IDDE03783BDCB147B9.ID38C90A6265D54EE8.png](media/IDDE03783BDCB147B9.ID38C90A6265D54EE8.png)

</td>

</tr>

<tr>

<td>![IDDE03783BDCB147B9.IDD8FA264C679C4B15.jpg](media/IDDE03783BDCB147B9.IDD8FA264C679C4B15.jpg)**Accumulative Time Balance**</td>

<td>

Contains functionality to accrue a value backwards or forwards in time. For example this function can be used to calculate remaining budget on a given time for a project period.

To add Accumulative Time Balance, right-click the value and select Accumulative Time Balance.

<span style="FONT-WEIGHT: bold; FONT-STYLE: italic">Reference period is set the time limit for the aggregation.  
<span style="FONT-WEIGHT: bold; FONT-STYLE: italic">Accumulate to set the operator < b less thanb  or <= b less than or equal tob .  
<span style="FONT-WEIGHT: bold; FONT-STYLE: italic">Lower boundary set the start time for the aggregation.  

<span style="FONT-WEIGHT: bold; FONT-STYLE: italic">![IDDE03783BDCB147B9.IDF8AF460E88944440.png](media/IDDE03783BDCB147B9.IDF8AF460E88944440.png)

</td>

</tr>

<tr>

<td>![IDDE03783BDCB147B9.ID52E1688722784365.jpg](media/IDDE03783BDCB147B9.ID52E1688722784365.jpg)  **Sort**</td>

<td>Sort the data in the table on the value you are trying to sort. This function is only available in when only one object is place in vertical axis or horizontal axis.</td>

</tr>

<tr>

<td>**Aggregation Method**</td>

<td>Set the aggregation method like sum, average, max, min, standard deviation, count and median for the value.</td>

</tr>

<tr>

<td>**Option for Explore**</td>

<td>Set the default target to explore.</td>

</tr>

<tr>

<td>**Hidden**</td>

<td>Hide the value in the report. For example you can hide a value used in a formula from beeing visible in the report. This function is only available when there is more than one values in the values field.</td>

</tr>

<tr>

<td>**Find**</td>

<td>Show a list over values in the values field.</td>

</tr>

<tr>

<td>**Remove**</td>

<td>Remove the value from the report.</td>

</tr>

</tbody>

</table>


## Naming Series Calculations

You can customize the name of a series calculation. You need only to change the name for the series calculation on one of the values in the report. Every value referencing to same data source, will inherit the customized name. Right-click the value and point to **Series Calculation** and then click available data source, to customize name on the series calculation. In the **Properties** tab and in the **Name** field, enter the new name.

![IDCED4C579FE4541BC.ID89C623FDD08445D1.png](media/IDCED4C579FE4541BC.ID89C623FDD08445D1.png)

To inherit the name from the aggregated data source, in the **Format** tab and in the <span style="FONT-WEIGHT: normal">Inherit Name field, click **Add after**.

![IDCED4C579FE4541BC.IDF1F44B09C95A47D4.png](media/IDCED4C579FE4541BC.IDF1F44B09C95A47D4.png)

**Tip:** Always customize the first value in the Value field. It is easier to remember which value that controls the customized name on series calculation.  

