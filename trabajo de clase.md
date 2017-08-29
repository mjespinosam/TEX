# Día uno

http://bit.ly/2wbCaJ9

Visual versus Semantic Encoding


Activity

1) With a pen or pencil, draw a box around examples of these data types and give each data type a “label”.

2) Figure out how many different kinds of data are on this page.

3) Identify or explain how these data types are communicated to you as a human reader.

4) Identify what kinds of relationships between data types are communicated and how is this communicated.

Question: Were there any data types or relationships presented in ambiguous or unclear ways? What made these features ambiguous?
What is XML and How to Use It
What is XML

XML stands for eXtensible Markup Language and it is a specific technology or tool designed to allow us to semantically describe a text, document, or any kind of structured information.
Styling with Cascading Style Sheets (CSS)

Because we have encoded our text semantically, we can now use this logic to programmatically style and restyle our text.

Styles can be added by linking a stylesheet to our XML document like so:

<?xml-stylesheet type="text/css" href="mystyles.css"?>
Activity 1) With a pen or pencil, draw a box around examples of these data types and give each data type a “label”. 2) Figure out how many different kinds of data are on this page. 3) Identify or explain how these data types are communicated to you as a human reader. 4) Identify what kinds of relationships between data types are communicated and how is this communicated. Question: Were there any data types or relationships presented in ambiguous or unclear ways? What made these features ambiguous?

XML Sistema independiente de marcado semántico.


<?xml version="1.0" encoding="UTF-8"?>
<?xml-stylesheet type="text/css" href="juana.css"?>

<Essay>
    <info>

        <title> La inteligencia de las flores fragmento </title>
        <author> Maurice Maeterlink </author>
        <year>1985 </year>
        <person gender="male"/>
    </info>

    <text>
        <heading> III </heading> 
    
     
        <p>   
            
            Esa necesidad de movimiento, ese apetito de espacio, en
            la mayor parte de las plantas, se manifiesta a la vez en la flor y en el fruto; o, en
            todo caso, no revela en él más que una experiencia, una previsión menos compleja. Al
            revés de lo que sucede en el reino animal, y a causa de la terrible ley de inmovilidad
            absoluta de la planta
            <categories> <semilladificultades> el primero y peor enemigo de la
                semilla es el tronco paterno. </semilladificultades> </categories>
              </p>
        
        <p> Nos
            encontramos en un mundo extraño, en que los padres, incapaces de cambiar de sitio, saben
            que están condenados a matar de hambre o a ahogar a sus vástagos. <semilladestino>Toda
                semilla que cae al pie del árbol o de la planta es perdida o germinará en la
                miseria. </semilladestino> <semillaestrategias>De ahí el inmenso esfuerzo para sacudir el yugo y
            conquistar el espacio.
                </semillaestrategias> <semillaestrategias>e ahí los maravillosos sistemas de diseminación, de propulsión,
            de aviación, que en todas partes encontramos en el bosque y en el llano, entre ellos,
            por no citar de paso más que algunos de los más curiosos: la hélice aérea o sámara del
            Arce, la bráctea del Tilo, la máquina de cernerse del Cardo, del Amargón y del Salsifí;
            los resortes explosivos del Euforbio; la extraordinaria pera surtidora de la Momórdica;
            y mil otros mecanismos inesperados y asombrosos</semillaestrategias>,<semillaestrategias> pues puede decirse que no hay semilla
                que no haya inventado algún procedimiento particular para evadirse de la sombra materna </semillaestrategias>
            </p>
        
    </text>
</Essay>



title {
    display:block; color:green;
    
}

p { 
display:block; color: blue; 

}

categories {
    display:block; color:#F781F3 ;
    
}

 What element should I use to encode a line in a poem?
 
 
# Dia dos

6.2 Components of the Verse Line

seg (arbitrary segment) represents any segmentation of text below the ‘chunk’ level.

>What element should I use to encode a new page and or a new column in a manuscript?

<msDesc (manuscript description) contains a description of a single identifiable manuscript or other text-bearing object.
The msDesc element has the following components, which provide more detailed information under a number of headings. Each of these component elements is further described in the remainder of this chapter.

msIdentifier (manuscript identifier) contains the information required to identify the manuscript being described.
head (heading) contains any type of heading, for example the title of a section, or the heading of a list, glossary, manuscript description, etc.
msContents (manuscript contents) describes the intellectual content of a manuscript or manuscript part, either as a series of paragraphs or as a series of structured manuscript items.
physDesc (physical description) contains a full physical description of a manuscript or manuscript part, optionally subdivided using more specialized elements from the model.physDescPart class.
history groups elements describing the full history of a manuscript or manuscript part.
additional groups additional information, combining bibliographic information about a manuscript, or surrogate copies of it with curatorial or administrative information.
msPart (manuscript part) contains information about an originally distinct manuscript or part of a manuscript, which is now part of a composite manuscript.
msFrag (manuscript fragment) contains information about a fragment of a scattered manuscript now held as a single unit or bound into a larger manuscript.


Question: What element (or elements) should I use to add an image?

<figure> groups elements representing or containing graphic information such as an illustration, formula, or figure. [14.4 Specific Elements for Graphic Images]
<figure>

14.4 Specific Elements for Graphic Images

The following special purpose elements are used to indicate the presence of graphic images within a document:

figure groups elements representing or containing graphic information such as an illustration, formula, or figure.
graphic indicates the location of a graphic or illustration, either forming part of a text, or providing an image of it.
binaryObject provides encoded binary data representing an inline graphic, audio, video or other object.
figDesc (description of figure) contains a brief prose description of the appearance or content of a graphic figure, for use when documenting an image without displaying it.
The graphic and binaryObject elements form part of the common core module, and are discussed in section 3.9 Graphics and Other Non-textual Components.

The figure element is used to contain images, captions, and textual descriptions of the pictures. The images themselves are specified using the graphic element, whose url attribute provides the location of an image. For example:

