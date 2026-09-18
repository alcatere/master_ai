En los datos de Géron, ¿por qué el codo “prefiere” (k = 4) si make_blobs usó 5 centros?
Porque en mi caso 2 blobs quedaron muy pegado, y el codo no puede distinguirlos, por lo que los considera como un solo cluster, y por eso el codo prefiere 4 clusters en lugar de 5.

Con tus blobs separados, ¿el codo y la silueta coinciden en el mismo (k)? ¿Ese (k) es 5?
En mi caso si, el codo y la silueta coinciden en k=4, son los que mejor valores dan, a pesar de que hayan sido 5 clusters.

Si el codo sigue en 4, ¿qué te falta mover (distancia entre centros vs. blob_std)?
Si se hubiera querido definir bien, deberia de haber movido mas los centroides de los blos y hacer el std mas pequeño.