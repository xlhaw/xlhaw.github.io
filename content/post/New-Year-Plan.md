---
title: "New Year Plan 2018"
date: 2018-02-20 09:18:00
tags:
- plan
- dot
- example
categories:
- lifestyle
description : "New Year Plan 2018"
cover : "/images/gci/gci-thumb.png"
draft: false
---
  <script type="text/javascript"
     src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
  </script>
<script src="http://cdnjs.cloudflare.com/ajax/libs/raphael/2.2.0/raphael-min.js"></script>
<script src="http://cdnjs.cloudflare.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
<script src="http://flowchart.js.org/flowchart-latest.js"></script>
<script src="https://d3js.org/d3.v5.js"></script>

***

Say hi,say bye!

Say goodbye to yesterday low-efficiency and embrace a brand-new, productive lifestyle.

Cliche as always. I don't recall how much blogs I have created before.But I'm sure this blog will last as long as I'm able to write. Consider this article as the debut of _**'I do'**_ new episode, as well as the end of _**'Hello World'**_ storyline.


## Criteria
- Forget about yourself, don't critize and judge your past.
- Be nice to every person in your life and be gratefull.
- Don't haste to the result,yet take your time in your mind.


Accept imperfection, as Rome isn't built in a day, but you have to take action now. The TOC and Themes do not work proper so far, I hope in next sprint those issue will be fixed.

		Failure is not horrible. What's horrible is that you believe this.


## Purpose

    Instead of struggling with the purpose of life, why don't you choose some attainable targets?

For the rest of 2018, I pick up a few subjects that requires more endeavour and research in order to build your own framework.

For General skills: 

- Python  
- German  
- Business  
- Spreech  
- Badminton  

For Engineering:

- Process
- Product
- Materials
- Project
- Quality

And for Specialty:

- [ ] Magnetic Recording
- [ ] Quantum Computing
- [ ] Nano-Fabrication
- [ ] Heterogeneous Catalysis
- [ ] Machine Learning


            
![Machine Learning](\\images\ml.png\)

## Envision

I believe that once upon a time, we all have a dream. Though how unrealistic it may look like now or we have forgotten it or unwillingly to take about it.

I believe in love though I never have such experience.

I believe in science, regardless I'm a slow learner.

Of course, I also believe in money, sadly I have neither capital nor business insight.

 
> "Life is not about waiting for the storm to pass. It's about learning to dance in the rain."

 
Anyway, let's just rock and roll.

## Function Test
Since I'm still not very familiar with Markdown grammar. Please ignore below contents.

```flow
st=>start: Start
op=>operation: Data Analysis
cond=>condition: Desicion Making
e=>End
st->op->cond
cond(yes)->e
cond(no)->op
```

Euler Equation
$$e^{i\pi}+1=0$$

`Roadmap`

- Presentation
	- Visualization
		- Interaction
			- Innovation

|I|Love|You|
| :---: | :---: | :---: |
| So | Do | I |
| Just | A | Joke |


<div id="diagram">Diagram will be placed here</div>
<script>
  var diagram = flowchart.parse('st=>start: Start:>http://www.google.com[blank]\n' +
                                'e=>end:>http://www.google.com\n' +
                                'op1=>operation: My Operation\n' +
                                'op2=>operation: Stuff|current\n' +
                                'sub1=>subroutine: My Subroutine\n' +
                                'cond=>condition: Yes \n' + // use cond(align-next=no) to disable vertical align of symbols below
                                'or No?\n:>http://www.google.com\n' +
                                'c2=>condition: Good idea|rejected\n' +
                                'io=>inputoutput: catch something...|request\n' +
                                '\n' +
                                'st->op1(right)->cond\n' +
                                'cond(yes, right)->c2\n' + // conditions can also be redirected like cond(yes, bottom) or cond(yes, right)
                                'cond(no)->sub1(left)->op1\n' + // the other symbols too...
                                'c2(true)->io->e\n' +
                                'c2(false)->op2->e'  //allow for true and false in conditionals
                                );
  diagram.drawSVG('diagram');
</script>