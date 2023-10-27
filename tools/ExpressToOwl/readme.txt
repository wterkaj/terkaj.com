|----------------|
|  ExpressToOwl  |
|----------------|

Developer: Walter Terkaj (walter.terkaj@itia.cnr , walter@terkaj.com)

Description: Tool to convert an EXPRESS schema into an OWL ontology

License: see ExpressToOwl_License.txt file

Programming language: C++ (IDE: Visual Studio 2010)

Tested Working environment: Windows 7


*** How to use ***
Launch the program "ExpressToOwl32.exe" from command line, adding the following arguments:
1. Input EXPRESS file
2. Output ontology file
3. Output Ontology URI
4. Repository path as relative to the application path [OPTIONAL, default=""]
5. Add Class Expression for WHERE rules (0/1) [OPTIONAL, default=1]
6. Add Class Expression for LIST cardinality constraints (0/1) [OPTIONAL, default=1]
7. Adopt LDWG decisions (0/1) [OPTIONAL, default=1]
8. Base URI for imported EXPRESS scehamas [OPTIONAL, default="http://www.terkaj.com/"]
9. Generate EXPRESS ontology (0/1) [OPTIONAL, default=0]
10. Output Ontology Version URI [OPTIONAL, default=Ontology URI]

Regarding point.5, the conversion pattern is presented in Terkaj and Sojic (2015).

Regarding point.7, the LDWG decisions are listed here:
http://www.buildingsmart-tech.org/future/linked-data/ifcowl/express-to-owl-conversion-procedure-proposed-recommendation
As an alternative, the proposal made in the paper Pauwels and Terkaj (2016) can be adopted.


*** Example ***
ExpressToOwl32.exe IFC4_ADD1.exp IFC4_ADD1.owl http://ifcowl.openbimstandards.org/IFC4_ADD1 IFC4_ADD1 1 1 1 http://www.iso.org/ 0




