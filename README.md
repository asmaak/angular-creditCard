for using reactive forms
1-import {ReactiveFormsModule} from '@angular/forms'; at app.module.ts
add at your component
2-import {FormGroup,FormControl} from '@angular/forms';
3- create name for form 
 cardForm = new FormGroup({
   name: new FormControl('')=>initial value for name 
 })
 4- at component html add form 
 <form [formGroup]="cardForm">
  <input type="text" name="name" formControlName="name">
</form>
<!-- for validation form  -->
add validator
import {FormGroup,FormControl,Validator} from '@angular/forms';
<!-- install mask  -->
https://www.npmjs.com/package/ngx-mask
<!-- another way to make mask -->
$ ng g class DateFormControl

