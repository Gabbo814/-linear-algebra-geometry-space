# Practice Set B: Applicazioni lineari e cambi di base

## Istruzioni
- Mostra passaggi e giustifica le scelte (metodo/teoria usata).
- Tagga gli errori concettuali nell’Error Log.

### Problemi
1) Sia T: R^3→R^2 definita da T(x,y,z) = (x+2y−z, 3x−y+4z).
   - a) Trova la matrice A di T rispetto alle basi canoniche.
   - b) Calcola ker(T) e Im(T). Indica dimensioni e verifica rank–nullità.

2) Sia S: R^2→R^2 con S(x,y) = (x+y, x−y).
   - a) Mostra che S è isomorfismo.
   - b) Trova la matrice di S nella base ortonormale B={u1,u2} con u1=(1,1)/√2, u2=(1,−1)/√2 (rotazione di 45°).

3) Cambio di base: nello spazio V=R^3, considera le basi
   - B = {(1,0,0),(0,1,0),(0,0,1)}, C = {(1,1,0),(0,1,1),(1,0,1)}.
   - a) Costruisci la matrice P che converte coordinate da B a C (cioè [v]_C = P [v]_B).
   - b) Verifica che P è invertibile e trova P^{-1}.

4) Applicazione lineare composizione
   - Date T(x,y)=(2x+y, x−y) e U(x,y)=(x+3y, −x+2y), calcola la matrice di U∘T e T∘U. Sono simili? Giustifica.

5) Proiezione ortogonale su sottospazio
   - U = span{(1,0,1), (0,1,1)} ⊂ R^3. Costruisci una base ortonormale di U con Gram–Schmidt, poi la matrice di proiezione P_U e calcola P_U v per v=(2,−1,3).

6) Matrice rappresentativa e cambio di base
   - Sia T: R^3→R^3 con matrice A in base canonica. Trova la matrice [T]_B in una base B qualunque e mostra che [T]_B = P^{-1} A P, dove P è il cambio di base da B alla base canonica.

7) Nucleo e immagine via sistemi
   - Per A=[[1,2,−1],[0,1,1],[2,3,0]], trova una base di N(A) e di Im(A). Indica ranghi e verifica rank+nullità.

8) Isometrie e matrici ortogonali
   - Sia Q = matrice di rotazione in R^2 di angolo θ. Mostra Q^T Q = I e che ⟨Qv,Qw⟩ = ⟨v,w⟩.

9) Applicazioni iniettive/suriettive
   - Sia T: R^3→R^3 con A=[[1,0,0],[0,1,1],[0,0,0]].
     a) T è iniettiva? suriettiva?
     b) Descrivi ker(T) e Im(T).

10) Coordinate rispetto a base non canonica
   - In V=R^2, base B={(2,1),(1,1)}. Trova le coordinate di v=(3,2) rispetto a B e verifica con ricostruzione v = α(2,1)+β(1,1).
