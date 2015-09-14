<span class="title-snippet">Token/line/score durations in ticks per quarter note.</span>

Durations can be expressed in ticks by giving the tpq value as an
argument to the duration functions:

```cpp
int tpq = infile.tpq();                           // 6 ticks per quarter note
infile.token(3, 1).getDuration(tpq).toInteger();  // 2 ticks for a triplet eighth note
infile[3].getDuration(tpq).toInteger();           // 1 tick for a triplet sixteenth note
infile.getDuration(tpq).toInteger();              // 18 ticks for three quarter notes
```
