Download Link: https://assignmentchef.com/product/solved-cs2400-homework-8-book-class-modifications
<br>
<strong><em>Book   Class   Modifications:           </em></strong>

<ul>

 <li>Overload the output operator         (&lt;&lt;)     to         print    a          book.   The     book   must            be        printed           in         the       following        format without           any      new            lines:</li>

</ul>

Title:   Problem Solving with C++, Author: Walter Savitch, Published: 2018




Write   a          C++     program         that     uses    the       <em>Book</em>    class    to         search,            delete, or add      books. Assume           that     the       library will      contain           up        to         15,000 books. A data     file       of         books  will      be        provided.        Read   the       books  and      store   them   into an        array/vector  of         <em>Books. </em>The     program         should ignore all        blank   lines.   Each    line in         the       file       is         of         the       format:




&lt;Title&gt;|&lt;Year&gt;|&lt;Authors&gt;




<strong>The     program        should           allow  the      user    to        do       any     of         the      following (using command      line     arguments). The     following       options          should           be available       to        the      user:   </strong>




Assuming        your    program         name   is         “a.out”,        the       command       to         access the library are      as        follows:




./a.out  [option] string




<strong>Options                      </strong>

<strong>            </strong>

-a        Search by author

-t        Search by title

-y        Search by year

-n        Add new book to the library the book must be saved to the file.

-d  Delete a book by title (<strong>title must match exactly and should be case insensitive</strong>) No option                search for any string in the title, year, or author.




<strong>Examples:     </strong>

./a.out -a “aDaMs”

./a.out -t “GALaXy”

./a.out -y “19”

./a.out -n “Problem Solving with C++|2018|Walter Savitch”

./a.out -d “Problem Solving with C++”

./a.out “C++”







Keep    in         mind   that     these   search options           might  produce          more   than    one Book.




<strong>You     may    use      any     function        or        library           discussed      in        class   or        in the      chapters        we       covered         from   your   textbook.      Do       not      use      any other  libraries        or        functions.      </strong>

<strong>            </strong>

<strong>Parsing          command      line     arguments    </strong>

<strong>            </strong>

In         C++     you      can      input   data     into     your    program         on        the       command       line (command      line      arguments).               You     can      capture           these   data     by        adding two parameters    to         your    main    program         as        follows:

int main (int argc, char **argv)

argc:             (argument      count) number          of         arguments      on        the       line,     including           the       name   of         the       program

argv:             (argument      vector)            list       of         c-style strings that     represent       all        the           arguments      including        the       name   of         the       program         (two           dimensional   array   of         characters).

For      example,         executing        the       command:

./a.out -a “douglas adams”

Assigns:

argc = 3

argv[0] will be “./a.out” argv[1] will be “-a” argv[2] will be “douglas adams”

Quotation       is         necessary       if          you      are      using   white   spaces within the       string.

<strong>Your   program        must   print   an       error  message        and     explanation  if          any     of the      following       happens:       </strong>

<ol>

 <li>Number of         arguments      is         less      than    2          or        more   than</li>

 <li>Invalid option is           Begins with     ‘-‘     and      is         not      one      of         the            options           above.</li>

 <li>File access error</li>

</ol>







<strong>Hints:</strong>

<ul>

 <li>Use the       third    constructor    of         the       <em>Book</em>    class    to         initialize          each      book   in         the       array/vector.</li>

 <li>Test your    program         with     a          small   file</li>

 <li>Implement one      option at         a</li>

 <li>Start</li>

</ul>








