# WebBrowserStorage
Web browser storage: Local Storage and Session storage code

## NOTES

NOTE(1): There are 6 x Local, and/or, Session storage properties/methods...  

          name - type            usage  
                                
        length - property        localSession.length  
       clear() - method          localSession.clear()  
         key() - method          key(indexNo)  
     getItem() - method          getItem(keyName)  
     setItem() - method          setItem(keyName,value)  
  removeItem() - method          removeItem(keyName)  

NOTE(1): You can read the item name using key();   
         but, you cannot change it's value using key();   
         to change the item value you have to use: setItem(key,value).  

NOTE(2): There are 2 ways to set an items value...  
         a> setItem(keyName,value)  
         b> setItem.keyName = value  
         ...method a is best when using a loop to read/set both item: keyName/value pairs;   
         because method b doesn't allow you to employ variables for keyName.  

NOTE(3): If the keyName is say, a; and, it's value is set to, 1.  
         then, you cannot save another item with that exact same keyName/value pair: a,1;  
         you will find that the 'unique' keyName/keyValue still remains unchanged/(not duplicated).  
         However, you can use the same keyName to change -(over write)- any previous value: (eg. a,2).   

NOTE(4): Although, you may write keyName/value pairs in any order you please: b,z,k,d,a;   
         whenever these items are printed out through using key()...  
         they will appear in strict 'alphabetical/(ASCII)' keyName order: a,b,d,k,z.    

NOTE(5): The data entered can be of multiple different types:   

         letter,a  
         letters,abc  
         num-letters,123abc  
         sentence = This is a sentence.  
         symbols,@!"'/\^&*()£%|  
         integerNum,1  
         floatNum,1.0  
         phoneNo,1111 222 3333  
         boolean,True/False  
         answer,yes/no  
         url,http://www.w3schools.com  
         -etc.     

         However, it's worth nothing that all data, including both:   
         'keyName,Value', is stored in the form of being 'strings'.  

NOTE(6): The web browser storage limit is set to: 5MB.  

NOTE(7): a> localStorage, lasts permanently; until both it's 'name/value' pair are, quite deliberately, cleared;  
            data may be cleared either: programatically/or else, through using web browser controls.  
         b> sessionStorage, is impermanent...lasting only up until when the web browser is closed/  
            nor will it's 'name/value' pairs be transferred over into a 'new' tab window.  

## Links

###Video tutorials

JavaScript Storage Interface sessionStorage localStorage Tutorial  / (Adam Khoury)  
https://www.youtube.com/watch?v=klLMeL7I4O0  

