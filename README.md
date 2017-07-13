# android-databinding-error-pattern

Conditions

 * Data binding library
 * Use 2-way binding (@={accepted})
 * Use multiple layout qualifier (e.g. layout and layout-h480dp)
 
Then, Data binding library produces wrong code so we cannot compile an app...

```
/Users/fkm/dev/DataBindingErrorPattern/app/build/generated/source/apt/debug/com/mokelab/demo/databinding/databinding/ActivityMainBindingImpl.java:39: error: not an enclosing class: ActivityMainBinding
            if ((com.mokelab.demo.databinding.databinding.ActivityMainBinding.this) != (null)) {
                                                                             ^
/Users/fkm/dev/DataBindingErrorPattern/app/build/generated/source/apt/debug/com/mokelab/demo/databinding/databinding/ActivityMainBindingImpl.java:39: error: illegal start of type
            if ((com.mokelab.demo.databinding.databinding.ActivityMainBinding.this) != (null)) {
                ^
/Users/fkm/dev/DataBindingErrorPattern/app/build/generated/source/apt/debug/com/mokelab/demo/databinding/databinding/ActivityMainBindingImpl.java:43: error: not an enclosing class: ActivityMainBinding
                com.mokelab.demo.databinding.databinding.ActivityMainBinding.this.setAccepted(callbackArg_0);
                                                                            ^
/Users/fkm/dev/DataBindingErrorPattern/app/build/generated/source/apt/debug/com/mokelab/demo/databinding/databinding/ActivityMainBindingH480dpImpl.java:39: error: not an enclosing class: ActivityMainBinding
            if ((com.mokelab.demo.databinding.databinding.ActivityMainBinding.this) != (null)) {
                                                                             ^
/Users/fkm/dev/DataBindingErrorPattern/app/build/generated/source/apt/debug/com/mokelab/demo/databinding/databinding/ActivityMainBindingH480dpImpl.java:39: error: illegal start of type
            if ((com.mokelab.demo.databinding.databinding.ActivityMainBinding.this) != (null)) {
                ^
/Users/fkm/dev/DataBindingErrorPattern/app/build/generated/source/apt/debug/com/mokelab/demo/databinding/databinding/ActivityMainBindingH480dpImpl.java:43: error: not an enclosing class: ActivityMainBinding
                com.mokelab.demo.databinding.databinding.ActivityMainBinding.this.setAccepted(callbackArg_0);
                                                                            ^
6 errors
```
