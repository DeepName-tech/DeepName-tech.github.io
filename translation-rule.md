### breakpoint_stmt
  
    "breakpoint"
    
### assign_stmt (assign_stmt: variable "=" rvalue)

if rvalue contains interface invoke:

    str = "assign a value to local variable" + target variable + "."
    str += caller + "invokes an interface method from interface " + className + "."
    str += "the method has name as " + methodName + ","
    str += "and has parameter types as "
    for paraType in paraTypes:
        str += paraType + ","
    str += "and is fed with parameter values as "    
    for paraValue in paraValues:
        str += paraValue + ","
    str += "and returns a value of type" + retType + "."
    str += "finally the returned value of type " + retType + "is assigned to " + target variable + "."
    
if rvalue contains static invoke:
    
    str = "assign a value to local variable" + target variable + "."
    str += caller + "invokes an static method from class " + className + "."
    str += "the method has name as " + methodName + ","
    str += "and has parameter types as "
    for paraType in paraTypes:
        str += paraType + ","
    str += "and is fed with parameter values as "    
    for paraValue in paraValues:
        str += paraValue + ","
    str += "and returns a value of type" + retType + "."
    str += "finally the returned value of type " + retType + "is assigned to " + target variable + "."
    
if rvalue contains virtual invoke:
    
    str = "assign a value to local variable" + target variable + "."
    str += caller + "invokes an virtual(instance) method from class " + className + "."
    str += "the method has name as " + methodName + ","
    str += "and has parameter types as "
    for paraType in paraTypes:
        str += paraType + ","
    str += "and is fed with parameter values as "    
    for paraValue in paraValues:
        str += paraValue + ","
    str += "and returns a value of type" + retType + "."
    str += "finally the returned value of type " + retType + "is assigned to " + target variable + "."
    
if rvalue contains special invoke:
    
    str = "assign a value to local variable" + target variable + "."
    str += caller + "invokes an special (init, private, inherited) method from class " + className + "."
    str += "the method has name as " + methodName + ","
    str += "and has parameter types as "
    for paraType in paraTypes:
        str += paraType + ","
    str += "and is fed with parameter values as "    
    for paraValue in paraValues:
        str += paraValue + ","
    str += "and returns a value of type" + retType + "."
    str += "finally the returned value of type " + retType + "is assigned to " + target variable + "."
