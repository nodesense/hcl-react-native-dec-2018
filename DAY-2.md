Whole table 10000 elements

T1 - Creating Virtual DOM, render called - 1000 ms
T2 - REACT DIFF - compare all 10000 items - 500 ms
T3 - PATCH the changes on real ui - <span>100.35 1 ms
T4 - GC (cleanup old V.dom) - 300 ms

1.8 sec

For  row 100 elements - COMPONENT
T1 - Creating Virtual DOM, render called - 10 ms
T2 - REACT DIFF - compare all 10000 items - 5 ms
T3 - PATCH the changes on real ui - <span>100.35 1 ms
T4 - GC (cleanup old V.dom) - 3 ms



19 ms



For  row 10 elements - COMPONENT
T1 - Creating Virtual DOM, render called - 1 ms
T2 - REACT DIFF - compare all 10000 items - .5 ms
T3 - PATCH the changes on real ui - <span>100.35 1 ms
T4 - GC (cleanup old V.dom) - .3 ms


<table> -- 10000 V.DOM elements, 100 rows
<tr> each row has got 100 v.dom
...
<span>100.35
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...
<tr>
...