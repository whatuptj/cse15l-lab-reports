# Java Command: Grep

> `grep -e`:

**Example 1:**

Path: `./technical/biomed`

Using `grep -e "Conclusion" rr74.txt`

Will return:

`Conclusion`

**Example 2:**

Path: `./technical/biomed`

Using `grep -e "hypoxia" rr74.txt`

Will return:

```
Severe sustained hypoxia causes pulmonary hypertension
        following severe hypoxia has been reported in rats [ 4, 13,
        the murine lung following hypoxia, with previous reports [
        upregulated following hypoxia and that this may account for
        hypoxia from birth and measured NOS mRNA and protein
          ambient conditions, hypobaric hypoxia (simulating an
          animals that were exposed to hypobaric hypoxia as
          increased following hypoxia, with a trend toward
          1.5-fold following hypoxia as compared with normoxic
          eNOS levels were increased following hypoxia, and the
          not increase following exposure to hypoxia. This was
          pulmonary circulation following hypoxia resulted in
          in animals exposed to hypoxia as compared with sea level
        severe hypoxia-induced pulmonary hypertension. The
        animals exposed to hypoxia during postnatal
        The pulmonary hypertension in mice exposed to hypoxia
        studies of 4 weeks of hypoxia in mature animals [ 9]. The
        due to hypoxia. This is further supported by Tyler
        which hypoxia increases eNOS expression is poorly
        understood because a hypoxia responsive element has not yet
        transcription factor activator protein-1 during hypoxia may
        hypoxia, the central role of eNOS in protecting against
        hypoxia. In the present study, however, the increase in
        iNOS protein levels in adult mice following hypoxia was
        of hypoxia and inflammation has previously been reported to
        hypoxia and inflammation [ 23]. Others have also reported
        The iNOS promoter contains a hypoxia responsive element,
        and the increase in iNOS transcription in hypoxia may be
        due to the transcription factor hypoxia-inducible factor-1α
        that alterations in redox state during hypoxia may also
        28, 29]. It is not known whether hypoxia interferes with
        hypoxia. We have recently reported that mice deficient in
        hypoxia [ 4], but we did not find an increase in lung nNOS
        in mice following hypoxia. Increased nNOS has been
        other rat vascular beds following hypoxia, other reports
        suggest that the increase in NOS following hypoxia may be
        hypoxia, which correlated with impaired
        in vivo , acute hypoxia caused
        hypoxia in rats, Sato
        2 . This suggests that hypoxia inhibited
        lung following hypoxia in mice is presently unknown.
        upregulation in the murine lung with severe hypoxia-induced
        hypoxia may lead to more severe pulmonary hypertension than
        that observed in mature mice exposed to hypoxia, and this
```
       
The `-e` command line option for `grep` takes in a pattern to search for in a .txt file. In the first example, only one line contained the word "Conclusion", but in the second example, there were many lines that contained the pattern "hypoxia".

> `grep -f`

**Example 1:**

Path: `./technical/biomed`

Let's say there is a file called `patterns.txt` in `biomed` that contains a line with `Abbreviations`

Using `grep -f patterns.txt rr74.txt`

Will return:

`Abbreviations`

**Example 2:**

Path: `./technical/biomed`

Let's say there is another file called `patterns2.txt` in `biomed` that contains lines with `Abbreviations`, `Conclusion`, and `quantitative`

Using `grep -f patterns2.txt rr74.txt`

Will return:

```
quantitative one-tube reverse-transcription PCR (Applied
          quantitative reverse-transcription PCR, was increased
          confirmed using quantitative image analysis (data not
        Conclusion
        Abbreviations
```
        
The `-f` command line option for `grep` takes in a file with lines to search for in another file. It is similar to `-e` but instead can take just a file name rather than many `-e` parameters to search for in a file.

> `grep -i`

**Example 1:**

Path: `./technical/biomed`

Using `grep -i "conclusion" rr74.txt`

Will return:

`Conclusion`

**Example 2:**

Path: `./technical/biomed`

Using `grep -i "cOnCluSiOn" rr74.txt`

Will return:

`Conclusion`

`grep -i` is just like normally searching for patterns in text, except ignore lettercases. In Example 1, `Conclusions` still returned even though a lowercase `conclusions` was passed as the parameter.

> `grep -v`

**Example 1:**

Path: `./technical/biomed`

Using `grep -v "e" rr74.txt`

Will return:

```



        Introduction
        pulmonary vasoconstriction. Chronic NOS inhibition did not
        NO is important in modulating basal pulmonary vascular









          antirabbit (nNOS, iNOS, and β-actin) for 45 min at 37°C.


          with A
          260 /A
          RNA.


          dilution; nNOS, Transduction N32030, 1:500 dilution),


          2 -, NO


          Statistical analysis
          statistically significant.




          P < 0.001).


          brain).


          3.5-fold (Fig. 3).


          shown).





        Discussion
        21].
        circulation.
        production of NO
        hypoxia in rats, Sato
        in vitro and


        Conclusion




```

**Example 2:**

Path: `./technical/biomed`

Using `grep -v "" rr74.txt`

Will return:

nothing

`grep -v` is like the opposite of `grep -e`. That is because `grep -v` returns all lines that DON'T include the pattern.

To find how all of these command line options worked, I used `man grep` in the command line, chat gpt, and my own brain. :)
