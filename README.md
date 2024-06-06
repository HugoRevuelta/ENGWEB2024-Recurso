# ENGWEB2024-Recurso
1 las alteraciones para que funcionase la base de datos, habia que realizar que las listas de Strings en vez de tener esta estructura "['a','b']" habria que cambiarlas para que fuesen asi y asi poder realizar las operaciones con ellas ["a","b"]
y para comprobar que funciono adjunto esto C:\Users\hugor\OneDrive\Escritorio\examenrecurso\ex1>docker cp dataset2.json mongoEW:/tmp
Successfully copied 40.9MB to mongoEW:/tmp

C:\Users\hugor\OneDrive\Escritorio\examenrecurso\ex1>docker exec -it mongoEW bash
root@e9d4bf64ac2c:/# mongoimport -d livros -c livros /tmp/dataset2.json --jsonArray
2024-06-06T14:00:46.348+0000    connected to: mongodb://localhost/
2024-06-06T14:00:49.350+0000    [###########.............] livros.livros        18.5MB/39.0MB (47.5%)
2024-06-06T14:00:51.405+0000    [########################] livros.livros        39.0MB/39.0MB (100.0%)
2024-06-06T14:00:51.405+0000    20000 document(s) imported successfully. 0 document(s) failed to import.

Las queries estan en la carpeta ex1 en txt
Y para la api para correrlo debes realizar un npm start y en la puerta 17000 hacer los distintas operaciones,
y despues para el segundo ejercicio en la puerta 17001 se realizan axios a la puerta 17000 para añadiendo pugs se puedan visualizar los datos de los livros.
