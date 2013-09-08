magic-tables
============

jQuery responsive tables plugin its a small plugin that allows you to give a responsive behavior for your tables.


Features
--------

- Make your tables responsive easily
- Select columns/headings you want to show or not
- Set a custom heading for rows in responsive mode based on templates
- Control responsive behavior based on viewport width
- Based on the Chirs Coyier responsive tables approach described <a href="http://css-tricks.com/responsive-data-tables/">here</a>
- Lightweigth plugin ~< 2kb

Usage
-----


- jQuery is required
- Download the plugin <a href="">magic-tables.min.js</a> js file
- Download the plugin <a href="">magic-tables.min.css</a> css file


Include both files in your project and simply call the magicTable plugin over a table:

`````javascript

<script type="text/javascript">
    jQuery('.mytable').magicTable();
</script>

`````

Options
-------

You can pass a diferent options to customize responsive behavior

- <b>responsiveWidth</b> <i>default: 1024</i>

Set the min viewport width that enables responsive behavior.

- <b>skipColumns</b> <i>default: []</i>

Array with columns index you want to skip in responsive mode, starting from 0.

i.e. if you want to hide the first and third column you have to pass [0,2]

- <b>displayLabels</b> <i>default: true</i>

Controls column heading display for all rows

- <b>skipLabels</b> <i>default: []</i>

Array with columns heads you want to skip in responsive mode, starting from 0.

- <b>customTitle</b> <i>default: ''</i>

A html template to create custom heading for each row.

If is set, a new column will be added and the beginning of each row using the specfic template. 

You can define simple templates like

`````html
<b>{0}</b>. 
`````

{0} will be replace for the column 0 value. 

You can reference any column, no matter if that column are in the skipColumns array. 
In fact, you may want to use this feature in combination with skipColumns to create custom heading for each row in responsive mode and hide referenced columns.

See <a href="http://magictables.androb.com/#custom-title">custom title example</a> in demo page to give a better idea. 



- <b>labelSeparator</b> <i>default: ':'</i>

Set separator between column heading and column value in responsive mode.

Demo
----

See some demos <a href="http://magictables.androb.com">here</a>