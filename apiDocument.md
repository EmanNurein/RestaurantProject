# Page 1

# List of city
  # https://localhost:9700/location

# List of restaurants
  # http://localhost:9700/restaurants

# List of restaurants wrt to city
  # http://localhost:9700/restaurants/?state_id=1

# List of MealType
  # http://localhost:9700/mealType

# list of cost 
  # http://localhost:9700/cost

# Page 2

# List of restaurant on basis of meal
  # http://localhost:9700/restaurants/?meal_id=1

# Filter on basis of cuisine
  # http://localhost:9700/restaurants/?cuisine_id=1

# Filter on basis of cost
  # https://localhost:9700/restaurants/?cost_id=

# page 3
# Details of restaurants
  # http://localhost:9700/details/25cb97d5a04689830994708

# Menu on basis of restaurants
  # http://localhost:9700/menu/?rest_id=1

# page 4
# Menu detail of item selected
  # (POST) > http://localhost:9700/menuItem
    (body)> [1,2] 

# Place Order
   # (POST) http://localhost:9700/placeOrder
      (body) 
        {
            "name": "Eman",
            "email": "eman@gmail.com",
            "address": "Almuhandseen Block No.30",
            "phone": "0912133448",
            "cost": 4000,
            "menuItem": [
                1,
                5
            ],
            "status": "pending"
        },
    
# page 5

# See all place order
   # http://localhost:9700/viewOrder

# Get order on basis of emailId
   # http://localhost:9700/viewOrder?eman@gmail.com

# Update order
   # (PUT) localhost:9700/updateOrder/625d255e5b5070060e2250db
     (body)  
            {
                "status":"Delivered",
                "cost":"1200"
            }

# Rest login Api 

# GetAllUser
   # (GET)  http://localhost:5000/api/auth/users

# Register
   # (POST)  http://localhost:5000/api/auth/register
      (body)
        {
            "name":"Nada",
            "email":"nada@gmail.com",
            "password":"nada2022",
            "phone":"91222212",
            "role":"user"
        }

# Login
   # (POST)  http://localhost:5000/api/auth/login
     (body) 
            {
                "email":"nada@gmail.com",
                "password":"nada2022"
            }
     (response)=> {auth:true,token:'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZ'}

# UserInfo
   # (GET) => http://localhost:5000/api/auth/userinfo
    (Header) => {'x-access-token':'token value from login'}







