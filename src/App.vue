<script setup>
import {InPlaceEditorComponent as EjsInplaceeditor} from
 '@syncfusion/ej2-vue-inplace-editor';

const textModel = {placeholder: 'Enter your name'};
const saveButton = {content: 'Save', cssClass: 'e-outline'};
const cancelButton = {content: 'Cancel', cssClass: 'e-outline'};
const popupSettings = {model: {position: 'BottomRight'}};

</script>

<template>
<div class="container">
<table>
  <tr>
    <td><b>Enter your name</b></td>
    <td>
      <ejs-inplaceeditor type="Text" :model="textModel"
      value="Andrew" :saveButton="saveButton"
      :cancelButton="cancelButton"
      :popupSettings="popupSettings"
      editableOn="EditIconClick"
      :showButtons= false disabled="true">
      </ejs-inplaceeditor>  
    </td>
  </tr>
</table>
</div>
</template>

<style>
@import "../node_modules/@syncfusion/ej2-base/styles/material.css";
@import "../node_modules/@syncfusion/ej2-buttons/styles/material.css";
@import "../node_modules/@syncfusion/ej2-inputs/styles/material.css"; 
@import "../node_modules/@syncfusion/ej2-popups/styles/material.css";
@import "../node_modules/@syncfusion/ej2-inplace-editor/styles/material.css";

.container {
  text-align:left;
  margin-bottom: 60%;
}
.e-inplaceeditor .e-editable-value-wrapper .e-editable-value {
  border-bottom: 2px dotted green;
  color: blue;
  font-size: 12px; 
}
</style>
