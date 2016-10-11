[Chart plugin for PencilBlue](http://pencilblue.org)
=====

##### A simple chart plugin

Installation and Setup
-----

1. Clone the chart-pencilblue repository into the plugins folder of your PencilBlue installation

```shell
   cd [pencilblue_directory]/plugins
   git clone https://github.com/raga2560/chart-pencilblue

```

2. Install the chart-pencilblue plugin through the manage plugins screen in the admin section (/admin/plugins).

3. Add the ^tmp_sales_by_month^ directive to any HTML template and the chart will be automatically loaded.

Note: If your pencilblue application has other angular.js modules, you need to inject chart module "chartpencilblueApp" into "pencilblueApp" like below

```
<script type="text/javascript">
 angular.module('pencilblueApp', ['chartpencilblueApp'])
.controller('PencilBlueController', function($scope) {
     ^angular_objects^
})

</script>
```