# XQuery Installation Guide

## Required Software

- **XML Database**: Native XML database with XQuery support:
  - **BaseX**: Open-source XML database and XQuery processor
  - **eXist-db**: Open-source native XML database
  - **MarkLogic**: Enterprise NoSQL database with XQuery support
- **XQuery Processor**: Standalone XQuery engines:
  - **Saxon**: Java-based XQuery and XSLT processor
  - **Zorba**: C++ XQuery processor
- **IDE/Editor**:
  - **VS Code**: With XQuery extensions
  - **oXygen XML Editor**: Commercial XML/XQuery IDE (recommended)
  - **Eclipse**: With XQuery plugins

## File Extensions

- `.xq` - XQuery source files
- `.xqy` - Alternative XQuery source file extension
- `.xquery` - Full XQuery source file extension
- `.xql` - XQuery library modules
- `.xqm` - XQuery module files
- `.xml` - XML data files
- `.xsd` - XML Schema Definition files
- `.dtd` - Document Type Definition files
- `.xsl` - XSLT stylesheet files
- `.config` - Configuration files for XQuery processors
- `.mxml` - MarkLogic XML files
- `.xpr` - oXygen XML project files

## Package Management

```bash
# Most XQuery installations use built-in module libraries
# External modules can be imported in XQuery files

# BaseX package management
basex -c "REPO INSTALL http://example.org/pkg/package.xar"

# eXist-db package management (using Package Manager app)
# Or use the command line:
java -jar exist-db-client.jar -u admin -P admin -x "repo:install('http://example.org/pkg/package.xar')"

# MarkLogic package management (using Management API)
curl -X PUT --digest --user admin:admin -H "Content-type: application/xml" \
  -d @package.xml http://localhost:8002/manage/v2/packages/install

# Saxon has no built-in package management
# You typically manage JAR files manually
```

## Running XQuery Programs

```bash
# Run XQuery with BaseX
basex -i data.xml query.xq

# Run XQuery with BaseX (standalone)
basex "for $i in 1 to 10 return $i"

# Run with eXist-db (using REST API)
curl -s --user admin:admin \
  "http://localhost:8080/exist/rest/db/path/to/query.xq"

# Run with Saxon (command line)
java -cp saxon.jar net.sf.saxon.Query -s:data.xml -q:query.xq

# Run with MarkLogic (using REST API)
curl -X POST --digest --user admin:admin \
  -H "Content-type: application/x-www-form-urlencoded" \
  -d "xquery=for $i in 1 to 10 return $i" \
  http://localhost:8000/v1/eval

# Run with Zorba
zorba -i query.xq -f

# Debug XQuery in oXygen XML Editor
# Open query.xq and use the debugger interface
```

## Common Libraries

- **Standard Functions**: XQuery 3.1 built-in functions
- **Math Library**: Mathematical functions (math:\*)
- **Array Library**: Array functions (array:\*)
- **Map Library**: Map functions (map:\*)
- **String Library**: String processing (fn:\*)
- **HTTP Client**: HTTP request functions (http:\*)
- **File Library**: File system operations (file:\*)
- **Cryptography**: Hash and encryption functions (crypto:\*)
- **ZIP**: ZIP file handling (zip:\*)
- **SQL**: SQL database integration (sql:\*)
- **Process**: Operating system process handling (proc:\*)
- **JSON**: JSON processing functions (json:\*)
- **CSV**: CSV processing (csv:\*)
- **Random**: Random number generation (random:\*)
- **XSLT Integration**: XSLT functions (xslt:\*)
- **Validation**: XML validation functions (validate:\*)
