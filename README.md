- 👋 Hi, I’m @sudharaniJSLT
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
sudharaniJSLT/sudharaniJSLT is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

I wanted to iterate the nested array and access the array values.I have tried below JSLT but is is not working for me.Can you help me on this.

++++++++++++++++JSLT+++++++++++

def range(length, list)
    if (size($list) < $length)
        range($length, $list + [size($list)])
    else
        $list

def zip(arr1, arr2)[
    for (range(size($arr1), []))[$arr1[.], $arr2[.]]]
	

{
    
    "requests": flatten(zip([
for (.) {
             
    "body": {
          "data": {
              "attributes": {
                "a" : .a,
                "b" : .b
              }
			} 

        }
       }
],


[
   for(..contacts){

 "body": {
                "data": {
                    "attributes": {
                        "contact": {
                            "code": "contact"
                        },
                        "contacts": {
                            "id": ..Id,
                            "contact id" : ..Contact_Id

                        }
                    }
                }
            }
        }]

))
}




+++++++++++++++++++++++++++input+++++++++++++++===



[
  {
     "a" :"12",
     "b" :"13", 
      "contacts": [
          {
              "Id": "1",
              "Contact_Id": "1234"
              
          },
          {
              "Id": "2",
              "Contact_Id": "877656554"
              
          },
{
              "Id": "3",
              "Contact_Id": "333333"
              
          }
      ]      
  },
  {
      
"a" :"12",
"b" :"13",   
"contacts": [
          {
              "Id": "4",
              "Contact_Id": "77777"
               },
{
              "Id": "5",
              "Contact_Id": "888888"
              
          },
          {
              "Id": "6",
              "Contact_Id": "9999999"
              
          }
      ]      
  }
]
