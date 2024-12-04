This is the conversion between Mathematica and TikZiT (https://github.com/tikzit/tikzit)   for handling graph visualization and computation.



## 1. graph from Mathematica to tikz

```
g = WheelGraph[20];
generateTikZCode[g, "scaled_graph_output.tikz"];
```


Output:
```
\begin{tikzpicture}[scale=1.0]
  \begin{pgfonlayer}{nodelayer}
\node [style=whitenode] (1) at (0.0, 0.0) {};
\node [style=whitenode] (2) at (-6.14213, 7.89141) {};
\node [style=whitenode] (3) at (-8.37166, 5.46948) {};
\node [style=whitenode] (4) at (-9.694, 2.45485) {};
\node [style=whitenode] (5) at (-9.96584, -0.825793) {};
\node [style=whitenode] (6) at (-9.15773, -4.01695) {};
\node [style=whitenode] (7) at (-7.35724, -6.77282) {};
\node [style=whitenode] (8) at (-4.75947, -8.79474) {};
\node [style=whitenode] (9) at (-1.64595, -9.86361) {};
\node [style=whitenode] (10) at (1.64595, -9.86361) {};
\node [style=whitenode] (11) at (4.75947, -8.79474) {};
\node [style=whitenode] (12) at (7.35724, -6.77282) {};
\node [style=whitenode] (13) at (9.15773, -4.01695) {};
\node [style=whitenode] (14) at (9.96584, -0.825793) {};
\node [style=whitenode] (15) at (9.694, 2.45485) {};
\node [style=whitenode] (16) at (8.37166, 5.46948) {};
\node [style=whitenode] (17) at (6.14213, 7.89141) {};
\node [style=whitenode] (18) at (3.24699, 9.45817) {};
\node [style=whitenode] (19) at (-0.00000000000000704481, 10.0) {};
\node [style=whitenode] (20) at (-3.24699, 9.45817) {};
  \end{pgfonlayer}
  \begin{pgfonlayer}{edgelayer}
\draw (1) to (2);
\draw (1) to (3);
\draw (1) to (4);
\draw (1) to (5);
\draw (1) to (6);
\draw (1) to (7);
\draw (1) to (8);
\draw (1) to (9);
\draw (1) to (10);
\draw (1) to (11);
\draw (1) to (12);
\draw (1) to (13);
\draw (1) to (14);
\draw (1) to (15);
\draw (1) to (16);
\draw (1) to (17);
\draw (1) to (18);
\draw (1) to (19);
\draw (1) to (20);
\draw (2) to (3);
\draw (2) to (20);
\draw (3) to (4);
\draw (4) to (5);
\draw (5) to (6);
\draw (6) to (7);
\draw (7) to (8);
\draw (8) to (9);
\draw (9) to (10);
\draw (10) to (11);
\draw (11) to (12);
\draw (12) to (13);
\draw (13) to (14);
\draw (14) to (15);
\draw (15) to (16);
\draw (16) to (17);
\draw (17) to (18);
\draw (18) to (19);
\draw (19) to (20);
  \end{pgfonlayer}
\end{tikzpicture}
```
![image](https://github.com/user-attachments/assets/bbc4dede-7a40-4817-91cb-3942f0021fe4)




## 2. graph from  tikz to Mathematica
```
SetDirectory[NotebookDirectory[]];
graph = ImportTikZGraph["scaled_graph_output.tikz"];
```
![image](https://github.com/user-attachments/assets/ee47b49a-7180-49d6-ba4e-eed628986055)




