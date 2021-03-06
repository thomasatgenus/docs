# Create a Data Aggregate

Use this effect to build aggregations from a base data source. A base data source consists of the measurements or metrics of a business process, for example, *sales volume* by *day* and *product*. The measures act as independent variables by which dimensional attributes are analyzed.

Aggregations are built from the base data source by changing the granularity on specific dimensions and aggregating up measures along these dimensions. The result of the aggregation is stored in one of your data sources.

For information on committing changes, adjusting transaction timeouts, running with elevated privileges, and supressing user notifications, see [Scope](../blocks/scope.md "Scope").

1.  In the **Name** box, optionally enter a name. The name is displayed in the action tree, if a name is not entered, a summary of the effect is displayed.
2.  In the **Description** box, optionally enter a description.
3.  Click the **General** tab.
4.  In the **Base Data** list, select the data source containing the base data for the aggregate. The base data source is not a part of your data sources, and you can choose among all Object Classes defined in your Directory.
5.  Click **Filter Data** to restrict the amount of data aggregated. Follow the instructions in the [step-by-step procedure](../../data-sources/specifying-a-data-filter-for-a-data-source.md "Specifying a Data Filter for a Data Source") on how to specify a data filter for a data source.
6.  In the **Data Aggregate** list, select which data source to populate with the aggregated data. If you select a data source of type **Object**, the aggregations can be saved to permanent storage. For information on committing changes, adjusting transaction timeouts, running with elevated privileges, and supressing user notifications, see [Scope](../blocks/scope.md).
7.  Click the **Dimensions** tab. For each dimension defined in the data aggregate, you must select which field from the base data source to use for aggregating up measures along this dimension.
8.  In the table, click the dimension for which you want to select a field, and then click **Modify**. In the **Select Field or Group** dialog box, select a field of the same data type as the dimension in the data aggregate. Note that you can select fields located in other data sources that is referred in the base data source. For example, your base data source contains *sales volume* by *day* and *product*. The data aggregate is defined as *sales volume* by *day* and *product category*, where *product category* is an attribute defined on *product*. To aggregate data along the *product category* dimension, expand the *product* field and select the *product category* field for the *product*. Calendar dimensions, such as year, quarter, month and day, can be aggregated from fields with data type **Calendar Time**. You can also aggregate values along fields with data type **String** or **Integer**, such as a product number.
9.  Click the **Measures** tab. For each measure defined in the data aggregate, you must specify which field from the base data source to use for calculating the measure.
10.  In the table, click the measure you want to calculate, and then click **Modify**.
11.  In the **Value** list, click **Select a field or group**. In the **Select Field or Group** dialog box, select a field from the base data source or a data source referred in the base data source.
12.  In the **Aggregation Function** list, select the statistical function to use when aggregating data for the selected field.