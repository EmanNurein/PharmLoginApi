# login Api 

# GetAllUser
        (GET) >> http://localhost:5000/api/auth/users

        (GET) >> https://Pharm-loginapp.herokuapp.com/api/auth/users

# Register
        (POST) >> http://localhost:5000/api/auth/register
        (Body) =>   
                {
                "name":"Sara",
                "email":"sara@gmail.com",
                "password":"sara@jan@2022",
                "phone":"0912321177",
                "role":"user"
                }
        (post) >> https://Pharm-loginapp.herokuapp.com/api/auth/register
        (Body) =>
                {
                "name":"Waleed",
                "email":"waleed@gmail.com",
                "password":"waleedjan",
                "phone":"0124242545",
                "role":"user"
                }

# Login
        (POST) => http://localhost:5000/api/auth/login
        (body)  =>  {
                        "email":"eman@gmail.com",
                        "password":"eman2022"
                }
        (response)=> {auth:true,token:'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9'}


        (POST) => https://Pharm-loginapp.herokuapp.com/api/auth/login
        (Body) =>   {
                        "email":"samah@hotmail.com",
                        "password":"123samah123"
                }
        (Response) => {"auth": true, "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9"}


# UserInfo
        (GET) => http://localhost:5000/api/auth/userinfo
        (Header) => {'x-access-token':'token value from login'}

        (GET) => https://Pharm-loginapp.herokuapp.com/api/auth/userinfo
        (Header) => {'x-access-token':'token value from login'}


