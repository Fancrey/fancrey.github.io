<link href="turing.css" rel="stylesheet"></link>

# Fancrey

[toc]

## Questions



For equation (12), why do you constrain $X = XW$? It needs to be explained in detail. And If $Z$ is a matrix related to the Laplacian matrix, I think it should be explained here, not in equation (18)

There seems to be some problems with the $\|W-Z+\frac{J_2}{2}\|_{F}^{2}$ term of equation (14). According to my experience, he should be $\|W-Z+\frac{J_2}{\mu}\|_{F}^{2}$, and the same problem appears in equations (15) and (16). 
$$
\begin{align}
&\left \langle J_2, W-Z \right \rangle +\frac{\mu}{2} \left \| W-Z \right \| _{F}^{2} \\
=& \frac{\mu}{2}Tr(\frac{2}{\mu}J_2^T(W-Z)+(W-Z)^T(W-Z))\\
=& \frac{\mu}{2}Tr(\frac{2}{\mu}J_2+W-Z)^T(W-Z))\\
=& \frac{\mu}{2}Tr(W-Z+\frac{J_2}{\mu}+\frac{J_2}{\mu})^T(W-Z+\frac{J_2}{\mu}-\frac{J_2}{\mu}))\\
=& \frac{\mu}{2}Tr((W-Z+\frac{J_2}{\mu})^T(W-Z+\frac{J_2}{\mu})-(W-Z+\frac{J_2}{\mu})^T\frac{J_2}{\mu}\\
&+\frac{J_2^T}{\mu}(W-Z+\frac{J_{2}}{\mu})-\frac{J_2^TJ_2}{\mu^2})\\
=& \frac{\mu}{2}\left \| W-Z+\frac{J_2}{\mu} \right \|_{F}^{2}-\frac{1}{2\mu}\|J_2\|_{F}^{2}
\end{align}
$$
In parameter selection, different regular terms usually affect each other, so I don't think it should fix other parameters and then select them. It's better to do it at the same time to ensure that the best parameters can be found

