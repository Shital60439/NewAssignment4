<template>
<div>
  <nav class="flex items-center justify-between flex-wrap bg-blue-700 p-6">
        <div class="flex items-center flex-shrink-0 text-white mr-6">
            <span class="font-semibold text-xl tracking-tight">Welcome To Home </span>
        </div>
        <div>
            <!-- <a href="#" class="flex justify-endinline-block text-sm px-4 py-2 leading-none border rounded text-white border-white hover:border-transparent hover:text-teal-500 hover:bg-white mt-4 lg:mt-0">LogOut</a> -->
            <NuxtLink to="/"
                class="flex justify-endinline-block text-sm px-4 py-2 leading-none border rounded text-white border-white hover:border-transparent hover:text-teal-500 hover:bg-white mt-4 lg:mt-0">
                About Us</NuxtLink>
        </div>
    </nav>


    <div class="border-2 border-black m-3 p-6 ">
        <div>
            <h1 class="font-semibold text-center text-2xl text-amber-400">Dashboard</h1>
           
        </div>        
       <div class="grid grid-cols-5 gap-5">
            <div class="p-6 max-w-sm rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
             <article class="font-medium text-black ">
               <p>Product Name:Nike shoes</p>
               <p>Price 20000</p>
               <p>Categar:shoes</p>
               <p>color:Black</p>
            </article>  
        </div>
        

        <div
            class="p-6 max-w-sm rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
               <article class="font-medium text-black ">
               <p >Product Name:Samsung Galaxy M32</p>
               <p>Price:14,999</p>
               <p>Categar:mobile</p>
               <p>color:sky blue</p>
            </article> 
        </div>

        <div
            class="p-6 max-w-sm rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
               <article class="font-medium text-black ">
              <p>Product Name:Bag Half Moon</p>
               <p>Price 1,500</p>
               <p>Categar:Bag</p>
               <p>color:Black</p>
            </article> 
        </div>

         <div
            class="p-6 max-w-sm rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
               <article class="font-medium text-black ">
             <p>Product Name:Dzert Kid bag</p>
               <p>Price 2000</p>
               <p>Categar:Bag</p>
               <p>color:Pink</p>
            </article> 
        </div>

         <div
            class="p-6 max-w-sm rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
               <article class="font-medium text-black ">
              <p>Product Name:Adidas shoes</p>
               <p>Price 30000</p>
               <p>Categar:shoes</p>
               <p>color:white</p>
            </article> 
        </div>

         <div
            class="p-6 max-w-sm rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
               <article class="font-medium text-black ">
              <p>Product Name:Reebok shoes</p>
               <p>Price 20000</p>
               <p>Categar:shoes</p>
               <p>color:Black</p>
            </article> 
        </div>


         <div
            class="p-6 max-w-sm rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
               <article class="font-medium text-black ">
              <p>Product Name:skecher shoes</p>
               <p>Price 20000</p>
               <p>Categar:shoes</p>
               <p>color:Blue</p>
            </article> 
        </div>

         <div
            class="p-6 max-w-sm rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
               <article class="font-medium text-black ">
               <p>Product Name:Vivo Y3</p>
               <p>Price 20,000</p>
               <p>Categar:Mobile</p>
               <p>color:Red</p>
            </article> 
        </div>

        <div
            class="p-6 max-w-sm rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
               <article class="font-medium text-black ">
              <p>Product Name:Oppo A16</p>
               <p>Price 13490</p>
               <p>Categar:mobile</p>
               <p>color:blue</p>
            </article> 
        </div>

        <div
            class="p-6 max-w-sm rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700">
               <article class="font-medium text-black ">
               <p>Product Name:Nick Bag</p>
               <p>Price 1,490</p>
               <p>Categar:Bag</p>
               <p>color:blue</p>
            </article> 
        </div>
        </div>
        </div>
        


        <div class="  grid grid-cols-2  ">
          <div class="border-black  border-2 m-8 p-8">  
            <form @submit="formSubmit" class="bg-gray-100 border-blue-400 rounded-lg border-2 px-12">
            <table>
                <h2 class="text-teal-900 text-xl font-bold pt-6">“Add Product” Form</h2>
                <hr />
                
                <label class="pt-10 py-10 " for="ProductName">Product Name:</label><br />
                <input type="text" v-model="user.ProductName" id="ProductName" name="ProductName" placeholder="" /><br /><br />
                
                <label for="Price">Price:</label><br />
                <input type="number" v-model="user.Price" id="Price" name="Price" placeholder="" /><br /><br />
                
                <label for="Category"> Category : </label><br />
                <input type="text" v-model="user.Category" id="Category" name="Category" placeholder=" " />
                <br /><br />
               
               <label for="text">Color: </label><br />
                <input type="text" v-model="user.Color" id="Color" name="Color" placeholder=" " />
                <br /><br />
                <div>
                    <button class="py-1 px-5 mr-5 bg-black hover:bg-blue-400 text-white font-bold text-center rounded-md mb-3" type="submit" @click="formSubmit"> Submit </button>
                    <button class="py-1 px-5 bg-black hover:bg-blue-400 text-white font-bold text-center rounded-md mb-3" type="reset"> Reset </button>
                </div>
            </table>
        </form>
        </div>
        <div class="border-black  border-2 m-8 p-8">
            
        <table class="list">
            <tr>
                <!-- <th class="px-4 border-black rounded-lg border-2">id</th> -->
                <th class="px-4 border-blue-400 rounded-lg border-4">ProductName..</th>
                <th class="px-4 border-blue-400 rounded-lg border-4">Price</th>
                <th class="px-4 border-blue-400 rounded-lg border-4">Category</th>
                <th class="px-4 border-blue-400 rounded-lg border-4">Color</th>
                <th class="px-4 border-blue-400 rounded-lg border-4">Action</th>
            </tr>
            <tr v-for="(item,index) in users" v-bind:index="index" :key="item">
                <!-- <td class="px-4 border-black rounded-lg border-2">{{item.id=i+1}}</td> -->
                <td class="px-4 border-blue-400 rounded-lg border-4">{{item.ProductName}}</td>
                <td class="px-4 border-blue-400 rounded-lg border-4">{{item.Price}}</td>
                <td class="px-4 border-blue-400 rounded-lg border-4">{{item.Category}}</td>
                <td class="px-4 border-blue-400 rounded-lg border-4">{{item.Color}}</td>
                <td class="px-4 border-blue-400 rounded-lg border-4">{{item.Action}}
                    <button class="mx-3 rounded-lg bg-red-600 hover:bg-red-700 text-white w-20" @click="userDelete(index)">
                        Delete
                    </button>
                    <button class="mx-3 rounded-lg bg-green-600 hover:bg-green-600 text-white w-20" @click="onEdit(index)">
                        Edit
                    </button>
                </td>
            </tr>
        </table>
        </div>
    </div>
    <div class="border-black  border-2 m-8 p-8">
          <h1 class="font-semibold text-center text-2xl text-amber-400"> Filter the Product based on added categories</h1>
            <div>
            <label class="font-bold text-xl mr-16" for="searchpro">Filter the Product</label>
            <input type="text" id="Productname" name="Productname" class="border-black  border">
        </div>
    </div>

    </div>

</template>
<script>
export default {
    data() {
        return {
            isEdit:false,
            indexEdit:-1,
            users: [],
            userAddress:'',
            user: {
                ProductName: '',
                Price: '',
                Category: '',
                Color: '',
            },
        };
    },
    methods: {
        formSubmit(event) {
            event.preventDefault();
            if(this.user.ProductName==""||this.user.ProductName==null||this.user.Price==""|| this.user.Price==null|| this.user.Category==""||this.user.Category==null|| this.user.Color==""||this.user.Color==null)
            {alert("please fill all the fields");
            this.onReset();
            
            }else{console.log("Hi");}
            if(this.isEdit==true){
                this.users[this.indexEdit]=this.user;
                this.isEdit=false;
                this.indexEdit=-1;
            }
            else{
                 this.users.push(this.user);
            }
           this.user = {
                ProductName: '',
                Price: '',
                Category: '',
                Color: '',
            };
        },
        onReset(event) {
            event.preventDefault();
            this.form.ProductName = "";
            this.form.Price = "";
            this.form.Category = "";
            this.form.Color = "";
           
        },
        userDelete(index) {
            this.users.splice(index, 1)
        },
        onEdit(index){
            this.user.ProductName=this.users[index].ProductName;
            this.user.Price=this.users[index].Price;
            this.user.Category=this.users[index].address;
            this.user.Color=this.users[index].Color;
            this.isEdit=true;
            this.indexEdit=index;
        },
    
         
    }
}
       
        
    
</script>