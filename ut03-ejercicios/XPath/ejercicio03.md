Ejercicio 3: Biblioteca Digital

<library>
  <book id="301">
    <title>The Catcher in the Rye</title>
    <author>J.D. Salinger</author>
    <genre>Fiction</genre>
    <available>true</available>
  </book>
  <book id="302">
    <title>To Kill a Mockingbird</title>
    <author>Harper Lee</author>
    <genre>Fiction</genre>
    <available>false</available>
  </book>
  <book id="303">
    <title>The Great Gatsby</title>
    <author>F. Scott Fitzgerald</author>
    <genre>Fiction</genre>
    <available>true</available>
  </book>
  <book id="304">
    <title>1984</title>
    <author>George Orwell</author>
    <genre>Dystopian</genre>
    <available>true</available>
  </book>
  <book id="305">
    <title>Moby Dick</title>
    <author>Herman Melville</author>
    <genre>Adventure</genre>
    <available>false</available>
  </book>
</library>

Preguntas:

01. Selecciona todos los títulos de los libros.

//book/title

2.  Selecciona todos los libros disponibles (con available="true").

//book[available="true"]

//book[available="true"]/title/text()


3.  Selecciona el autor del libro "1984".

//book[title="1984"]/author

//book[title="1984"]/author/text()

4.  Selecciona todos los géneros de libros únicos.

//book/genre[not(. = preceding-sibling::genre)]

//book/genre[not(. = preceding-sibling::genre)]/text()

5.  Cuenta cuántos libros están disponibles.

count(//book[available="true"])

6.  Selecciona los títulos de los libros que no están disponibles.

//book[available="false"]/title/text()

7.  Selecciona los autores cuyos libros están disponibles.

//book[available="true"]/author/text()

8.  Selecciona el ID del libro "The Great Gatsby".

//book[title="The Great Gatsby"]/@id

9.  Selecciona todos los libros del género "Fiction".

//book[genre="Fiction"]

//book[genre="Fiction"]/title/text()

10. Selecciona los títulos de los libros cuyo autor es "Herman Melville".

//book[author="Herman Melville"]/title/text()