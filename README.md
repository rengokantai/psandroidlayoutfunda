# psandroidlayoutfunda
##1. Introduction
###1 Basic Layouts
LinearLayout:align children in single direction.  
RelativeLayout(sometimes this can be achieved by nested LinearLayout, but affect performance)  
TableLayout: vertical LinearLayout nested horizontal LinearLayout

###3 Size
dp: density-independent pixel
px = dp*density  
density = bucket(dpi/160)


###4 Margin vs Padding
```
android:layout_margin
android:padding="16dp"
```

###5 Gravity
```
android:gravity  // itself
android:layout_gravity  //parent container
```
Ex
```
<TextView android:layout_gravity="center_horizontal"/> //move all container
<TextView android:gravity="center_horizontal"/>  //only move text
```

more than one
```
android:gravity="center_horizontal|bottom"
```
