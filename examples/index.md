# calendar

---

````iframe:250
<div class="row">
  <input type="text" />
</div>
<div class="row">
  <input id="date" type="text">
</div>

<script>
seajs.config({
  locale: 'zh-cn',
  preload: ['seajs/plugin-i18n']
});

seajs.use(['$','date-picker'], function($,DatePicker) {
  new DatePicker({
    target: '#date'
  });
});
</script>
````

##auto-render

````iframe:250
<input id="date" type="text" data-widget="date-picker">

<script type="text/javascript">
seajs.config({
  locale: 'zh-cn',
  preload: ['seajs/plugin-i18n']
});

seajs.use(['widget'], function(Widget) {
  Widget.autoRenderAll();
});
</script>
````
