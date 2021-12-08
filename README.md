# Handeling String

## Creation
--------------

String is an object that represents sequence of characters. In Java, String is represented by String class which is located into java.lang package

It is probably the most commonly used class in java library. In java, every string that we create is actually an object of type String. One important thing to notice about string object is that string objects are immutable that means once a string object is created it cannot be changed.

**String can be Created as:**

```java
char[] s={'P','r','a','s','h','a','n','t'};  
```
```java
String s = "Prashant";  
```
```java
String s = new String("Prashant")
```

## Concatination and Conversion of String
-----------------------------------------
### Concatination of String:
In Java, String concatenation forms a new String that is the combination of multiple strings. There are two ways to concatenate strings in Java:

#### **By + (String concatenation) operator**
Java String concatenation operator (+) is used to add strings.

**Example**
```Java
public class string {
    public static void main(String[] args) {
        String s="Prashant"+"Bhandari";
        System.out.println(s);
    }
}
```

#### **By ``concat()`` method**
The String ``concat()`` method concatenates the specified string to the end of current string. 

Syntax:
```Java
public String concat(String another)  
```

Example:
```Java
public class string {
    public static void main(String[] args) {
        String s1="Prashant";
        String s2="Bhanadari";
        System.out.println(s1.concat(s2));
    }
}
```
### Conversion of String:
We can convert String to an int in java using ``Integer.parseInt()`` method. To convert String into Integer, we can use ``Integer.valueOf()`` method which returns instance of Integer class.

## Changing case in string
-----------------------------------

We can change case using :

* ``toLowerCase()`` for uppercase string
* ``toUpperCase()`` for lowercase string

```Java
String txt = "Hello World";
System.out.println(txt.toUpperCase());
System.out.println(txt.toLowerCase());
```
## Character Extraction 
-----------------------------------

There are several ways by which characters can be extracted from String class object. String is treated as an object in Java so we can’t directly access the characters that comprise a string. For doing this String class provides various predefined methods.

* ``char charAt(int index)``
* ``void getChars(int stringStart, int stringEnd, char arr[], int arrStart)``
* ``byte [] getBytes()``
* ``char [] toCharArray()``

## String Comparision 
-------------------------------
There are three ways to compare String in Java:

* **By Using ``equals()`` Method**:The String class equals() method compares the original content of the string. It compares values of string for equality. String class provides the following two methods:

    * ``public boolean equals(Object another)``: compares this string to the specified object.
    * ``public boolean equalsIgnoreCase(String another)``: compares this string to another string, ignoring case.

* **By Using ``==`` Operator**

* **By ``compareTo()`` Method**

    * ``s1 == s2``: The method returns 0.
    * ``s1 > s2`` : The method returns a positive value.
    * ``s1 < s2`` : The method returns a negative value.

## Searching String:


<table>
<th class="thStyle">Syntax</th>
<th class="thStyle">Explanation</th>
</tr>
<tr class="trStyle">
<td class="tdStyle"><div class="bold-font"><i>int indexOf(char ch)</i></div></td>
<td class="tdStyle">This method will return the index of the first occurrence of a character  variable <code class="code">ch</code> in the invoked string.</td></tr>
<tr class="trStyle"><td class="tdStyle"><div class="bold-font"><i>int lastIndexOf(char ch)</i></div></td>
<td class="tdStyle">This method will return the index of the last occurrence of a character variable <code class="code">ch</code> in the invoked string.</td></tr>
<tr class="trStyle"><td class="tdStyle"><div class="bold-font"><i>int indexOf(String st)</i></div></td>
<td class="tdStyle">This method will return the index of the first occurrence of a <code class="code">substring st</code> in the invoked string.</td></tr>
<tr class="trStyle"><td class="tdStyle"><div class="bold-font"><i>int lastIndexOf(String st)</i></div></td>
<td class="tdStyle">This method will return the index of the last occurrence of a <code class="code">substring st</code> in the invoked string.</td></tr>
<tr class="trStyle"><td class="tdStyle"><div class="bold-font"><i>int indexOf(char ch, int startIndex) <br>int indexOf(String st, int startIndex)</i></div></td>
<td class="tdStyle">Here <code class="code">startIndex</code> specifies the starting point of search. The search runs from <code class="code">startIndex</code>to end of the String.</td></tr>
<tr class="trStyle"><td class="tdStyle"><div class="bold-font"><i>int lastIndexOf(char ch, int startIndex) <br>int lastIndexOf(String st, int startIndex)</i></div></td>
<td class="tdStyle">Here <code class="code">startIndex</code> specifies the starting point of search. The search runs from <code class="code">startIndex</code> to zero.</td></tr></table>

## String Buffer

Java StringBuffer class is used to create mutable (modifiable) String objects. The StringBuffer class in Java is the same as String class except it is mutable i.e. it can be changed.
