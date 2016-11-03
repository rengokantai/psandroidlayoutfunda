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

##2. LinearLayout
###2 Gravity
in horizontal, the `layout_gravity` can only be top and bottom.
in veritcal, the `layout_gravity` can only be left and right.


###3 Weight
```
<LinearLayout ....
<TextView android:layout_width="0dp" android:layout_weight="1" ...
<TextView android:layout_width="0dp" android:layout_weight="2" ...
</LinearLayout>
```

####05:04 Dummy views, center a TextView
```
<LinearLayout>
<View android:layout_weight="1"
<TextView android:layout_weight="1"
<View android:layout_weight="1"
</LinearLayout>
```
####06:06 weightSum
Hence the previous example is same as
```
<LinearLayout android:gravity="center_horizontal" android:weightSum="3">
<TextView android:layout_weight="1"
</LinearLayout>
```
