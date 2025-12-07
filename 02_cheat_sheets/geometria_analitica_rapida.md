# Geometria analitica rapida (formule e criteri)

## Rette e piani in R^3
- Piano: a x + b y + c z + d = 0; vettore normale n=(a,b,c).
- Retta: forma parametrica r(t)=p+td, con punto p e direzione d.
- Parallelismo: r ∥ π ⇔ ⟨d,n⟩=0; r ⊂ π ⇔ ⟨d,n⟩=0 e p soddisfa π.
- Perpendicolarità: r ⟂ π ⇔ d ∥ n.
- Angolo tra piani: cosθ = |n1·n2|/(||n1||·||n2||).
- Intersezione di due piani: direzione = n1×n2; trova un punto risolvendo il sistema lineare.

## Distanze
- Punto‑piano: dist(P,π)=|a x_0 + b y_0 + c z_0 + d| / √(a^2+b^2+c^2), con P=(x_0,y_0,z_0).
- Punto‑retta: sia r(t)=p+td; dist(P,r)=|| (P−p) − proj_d(P−p) || = || (P−p) − ((P−p)·d/||d||^2) d ||.
- Distanza tra rette sghembe r1: p1 + t d1 e r2: p2 + s d2:
  d = | ( (p2−p1) · (d1 × d2) ) | / || d1 × d2 ||, se d1 × d2 ≠ 0.

## Angoli
- Angolo tra rette: cosθ = |d1·d2|/(||d1||·||d2||).
- Angolo tra retta e piano: sinθ = |d·n|/(||d||·||n||) (θ è l’angolo acuto tra la retta e il piano).
- Angolo tra piani: vedi sopra con i normali.

## Forme di rappresentazione
- Retta (R^3):
  - Parametrica: r(t)=p+td.
  - Cartesiana: sistema di due equazioni lineari (intersezione di piani).
- Piano (R^3):
  - Cartesiana: a x + b y + c z + d = 0.
  - Parametrica: π: p + s u + t v (u,v indipendenti e non collineari).
  - Forma normale: ⟨n, x⟩ = δ (con δ=−d se n è unitario).

## Coniche (R^2) e quadriche (R^3)
- Forma matriciale (2D): q(x)=x^T A x + l^T x + f, con A simmetrica.
  - Classificazione metrica tramite autovalori di A:
    - Ellisse: entrambi gli autovalori > 0 (forma definita positiva).
    - Iperbole: autovalori di segni opposti (forma indefinita).
    - Parabola: un autovalore 0 e l’altro > 0 (forma semidefinita).
  - Riduzione in forma canonica: rotazione (diagonalizzazione ortogonale di A) + traslazione (completamento del quadrato).
- Quadriche (3D): Q(x)=x^T A x + l^T x + f.
  - Classificazione tramite segnatura di A e termini lineari:
    - Ellissoide: A definita positiva, forma centrata (l=0 o assorbibile) ⇒ sezioni ellittiche.
    - Cono: forma indefinita senza termini lineari dominanti.
    - Cilindro: presenza di autovalore 0 e assenza di termine lineare lungo la direzione nulla.
    - Paraboloidi (ellittico/iperbolico): uno o più autovalori 0 con termini lineari non eliminabili completamente.

## Operazioni pratiche
- Completamento del quadrato (2D):
  1) Centrare: x = y + c, con c = −(1/2) A^{-1} l (se A invertibile).
  2) Diagonalizzare la parte quadratica: A = Q Λ Q^T (Q ortogonale).
  3) Nuove coordinate: y' = Q^T y per rimuovere i termini misti.
- Riduzione congruente (3D):
  - Esiste P invertibile tale che P^T A P = D (diagonale con ±1 e 0) mantenendo la segnatura (teorema di Sylvester).

## Criteri rapidi
- Compatibilità Ax=b (Rouché–Capelli): rank(A) = rank([A|b]).
- Unicità/infinite soluzioni: unica se rank(A)=n; infinite se rank(A)<n (compatibile).
- Diagonalizzabilità (endomorfismi):
  - Sufficiente: n autovettori indipendenti; per matrici simmetriche reali: sempre diagonalizzabili ortogonalmente.
- Proiezione ortogonale su U = span{q1,…,qk} con {q_i} ortonormali: P_U = Q Q^T, Q=[q1 … qk].

## Note di calcolo
- Uso del prodotto vettoriale: d_intersezione = n1 × n2, ||n1 × n2|| misura il seno dell’angolo tra i piani.
- Stabilità numerica: preferisci forme ortonormali (Gram–Schmidt) e RREF per lettura chiara dei pivot; attento al condizionamento (SVD: κ=σ_max/σ_min).
