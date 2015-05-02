# backtrace_llk_parser
a backtrace llk parser frame work in python, used to resolve certain semantic rulse,details in code
rulse

stat --> list EOF | assign EOF ;  //here the backtrace coming to use
assign --> list '=' list ;
list --> '[' elements ']' ; // match bracketed list
elements --> element (',' element)* ; // match comma-separated list
element  --> NAME '=' NAME | NAME | list ; //element is name, nested list



