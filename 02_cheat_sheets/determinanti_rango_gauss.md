# Determinanti, Rango, Gauss/Gauss–Jordan (Cheat Sheet)

## Determinante
- Proprietà: det(AB)=det(A)det(B); det(A^T)=det(A); det(A)≠0 ⇔ A invertibile.
- Effetto di operazioni di riga: scambio di righe → cambia segno; moltiplicazione di una riga per k → moltiplica det per k; somma di multipli di riga → det invariato.
- Interpretazione geometrica: fattore di scala di area/volume; orientazione. (Binet: det(AB)=det(A)det(B)).

## Rango
- rank(A) = numero di pivot in forma ridotta; dim(col(A)) = dim(row(A)).
- Teorema di Rouché–Capelli: sistema Ax=b compatibile ⇔ rank(A)=rank([A|b]); se compatibile, soluzioni: uniche ⇔ rank(A)=n; infinite ⇔ rank(A)<n.

## Gauss/Gauss–Jordan
- Gauss: riduzione a forma echelon (REF) per individuare pivot e risolvere Ax=b.
- Gauss–Jordan: riduzione a forma ridotta (RREF) per ottenere soluzioni esplicite e A^{-1} quando esiste.
