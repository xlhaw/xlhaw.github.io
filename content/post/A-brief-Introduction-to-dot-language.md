---
title: "A brief Introduction to DOT language"
date: 2018-03-17 20:58:30
tags:
- graphviz
- dot
categories:
- tools
description : "A brief Introduction to DOT language "
cover : "/images/gci/gci-thumb.png"
draft: false
---

# Free from Restrictions

I have been quite obesssed with fancy tools and techniques. Before I encounter with DOT, I have tried many tools to  reorganize my thought. Such as Visio,Grapholite,SimpleMind, Xmind, MindNode, iMindMap barabara, such a long list. All the software has its charming part and restrictions, but it's annoying to finetune for the position and format for a perfectionist or OD pa. Free yourself from the trival matter, you just need to focus on your own thinking, for,just like markdown help your the we, the dot help your .you can edit it anyway with a simple text edit such notpad or vim


The DOT language is really simple, use **->** symbol to shows the relationship between two objects and to modify any objects by change the value in [].
```
Object1 -> Object2
Object[Attribute=value]
```

The way it addresses the complex structures is also easy.  With **|** & _**{}**_, different elements are seperated and aggregated hierarchy. Specific label can also be accessed by put index<n> before it.

		Label [shape=record,label="<n>Label|{angle|distance|float|..}",labelangle=-60];
  

Find from the document [ojiji](www.)
​		  

You can even try it on lo from [vis.js](http://viz-js.com)


for more complicated case, 

![DOT Learning Note](..\\images\note.svg)

Learning by coding.

Here is the code.

```
digraph DOT {
compound=true;
DOT [label="DOT Languange"]
subgraph cluster0 {
label="Objects"
Nodes[label="Node"];
Edges[label="Edge"];
Edges -> Arrowhead;
Port [shape=record,label="{{nw|n|ne}|{w|<f0> Port|e}|{sw|s|se}}",headport=e];
Nodes -> "Port":f0;
Nodes -> Shape;
Shape [shape=record,label="{<f0>Shape|{<f1>box|<f2>invtriangle|<f3>ellipse}|{<f4>polygon|<f5>diamond|<f6>triangle}}"];
}
DOT -> Edges[label="Edge"];
DOT -> {Nodes,Generic,Advance};
subgraph cluster1 {
label="Attributes"
Advance -> {Font,Label};
Generic -> Color:n;
Generic -> Style:n;
Generic -> Size:n;
Label [shape=record,label="<n>Label|{angle|distance|float|..}",labelangle=-60];
Color [shape=record,label="<n>Color|{red|green|blue|..}",color=blue];
Style [shape=record,label="<n>Style|{<f0> dotted |<f1>bold|<f2>filled|..}",style=filled];
Size [shape=record,label="<n>Size|{<f0>height |<f1>width|<f2>weight|<f3>ratio|<f4>..}",style=bold,weight=0.8];
Font [shape=record,label="<n>Font|{name|color|size}",fontname=arial,fontcolor=Red];
Label -> Font[arrowhead=none];
}
subgraph cluster2 {
Cluster
}
Cluster -> Nodes[ltail=cluster2,lhead=cluster0,style=dotted,arrowhead=none];
Cluster -> Generic[lhead=cluster1,style=dotted,arrowhead=none];
Cluster -> triangle[lhead=cluster3,style=dotted,arrowhead=none];
subgraph cluster3 {
label="Instance";
box[shape=box];
ellipse[shape=ellipse];
polygon[shape=polygon];
diamond[shape=diamond];
triangle[shape=triangle];
color=lightgrey;
}
Shape:f1 -> box[label="dot",arrowhead=dot,style=dotted];
Shape:f3 -> ellipse[label="odot",arrowhead=odot,style=dotted, tailport=s];
Shape:f4 -> polygon[label="inv",arrowhead=inv,style=dotted,tailport=s];
Shape:f5 -> diamond[label="invdot ",arrowhead=invdot,style=dotted,tailport=s];
Shape:f6 -> triangle[label="invodot ",arrowhead=invodot,style=dotted];
Arrowhead -> box [lhead=cluster3,style=dotted,arrowhead=none];
}

```

At you the, it's time to your masterpiece, 

The final step is to render your masterpiece, After setup the enviorment variables properly,

tha the the cmd

	dot -Tsvg note.gv -o note.svg



Last but not the least

The language has done the trivial and dirty part, now is your turn to shine.

That's why many people embrace the open source software.