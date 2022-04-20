# login Api d

# GetAllUser
(GET)> http://localhost:5000/api/auth/users

# Register
(POST)> http://localhost:5000/api/auth/register
(body) =>  {
        "name":"Sara",
        "email":"sara@gmail.com",
        "password":"sara@jan@2022",
        "phone":"0912321177",
        "role":"user"
    }

# Login
(POST) => http://localhost:5000/api/auth/login
(body)  =>  {
            "email":"eman@gmail.com",
            "password":"eman2022"
            }
(response)=> {auth:true,token:'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9'}

# UserInfo
(GET) => http://localhost:5000/api/auth/userinfo
(Header) => {'x-access-token':'token value from login'}


