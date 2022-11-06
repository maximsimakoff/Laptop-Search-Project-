/*----------------------------------------------------------------------------------*/

/* 
                                  Laptop Picker
  The purpose of this app is to make it easy to find your laptop of choice by browsing 
  a selection of prices such as Low-Range, Mid-Range and Ultimate range. Every laptop
  is in a specific range based on price.

*/

/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
//Variables from Table/Data-set
var na = getColumn("Laptops", "name");
var price = getColumn("Laptops", "price");
var res = getColumn("Laptops", "resolution");
var mem = getColumn("Laptops", "memory");
var cpu = getColumn("Laptops", "cpu");
var gpu = getColumn("Laptops", "gpu");
var storage = getColumn("Laptops", "storage");
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
//Bubble-Sort Algorithm
function sort_name() {
  var temp_na;
  var temp_price;
  var temp_res; 
  var temp_mem;
  var temp_cpu;
  var temp_gpu;
  var temp_storage;

  for(var i = 0; i < na.length; i++){
     
   // Last i elements are already in place  
   for(var j = 0; j < ( na.length - i -1 ); j++){
       
     // Checking if the item at present iteration 
     // is greater than the next iteration
     if(na[j] > na[j+1]){
         
       // If the condition is true then swap them
       temp_na = na[j];
       na[j] = na[j + 1];
       na[j+1] = temp_na;
       
       temp_price = price[j];
       price[j] = price[j + 1];
       price[j+1] = temp_price;
       
       temp_res = res[j];
       res[j] = res[j + 1];
       res[j+1] = temp_res;
       
       temp_mem = mem[j];
       mem[j] = mem[j + 1];
       mem[j+1] = temp_mem;
       
       temp_cpu = cpu[j];
       cpu[j] = cpu[j + 1];
       cpu[j+1] = temp_cpu;
       
       temp_gpu = gpu[j];
       gpu[j] = gpu[j + 1];
       gpu[j+1] = temp_gpu;
       
       temp_storage = storage[j];
       storage[j] = storage[j + 1];
       storage[j+1] = temp_storage;
     }
   }
  }
}
function sort_price(printMessage) {
  var temp_na;
  var temp_price;
  var temp_res; 
  var temp_mem;
  var temp_cpu;
  var temp_gpu;
  var temp_storage;

  for(var i = 0; i < price.length; i++){
     
   // Last i elements are already in place  
   for(var j = 0; j < ( price.length - i -1 ); j++){
       
     // Checking if the item at present iteration 
     // is greater than the next iteration
     if(price[j] > price[j+1]){
         
       // If the condition is true then swap them
       temp_na = na[j];
       na[j] = na[j + 1];
       na[j+1] = temp_na;
       
       temp_price = price[j];
       price[j] = price[j + 1];
       price[j+1] = temp_price;
       
       temp_res = res[j];
       res[j] = res[j + 1];
       res[j+1] = temp_res;
       
       temp_mem = mem[j];
       mem[j] = mem[j + 1];
       mem[j+1] = temp_mem;
       
       temp_cpu = cpu[j];
       cpu[j] = cpu[j + 1];
       cpu[j+1] = temp_cpu;
       
       temp_gpu = gpu[j];
       gpu[j] = gpu[j + 1];
       gpu[j+1] = temp_gpu;
       
       temp_storage = storage[j];
       storage[j] = storage[j + 1];
       storage[j+1] = temp_storage;
     }
   }
  }
   if(printMessage == true){
    console.log("Data sorted!");
  }
  else if(printMessage == false){
    console.log("Data NOT sorted!");
  }
}
function sort_res() {
  var temp_na;
  var temp_price;
  var temp_res; 
  var temp_mem;
  var temp_cpu;
  var temp_gpu;
  var temp_storage;

  for(var i = 0; i < res.length; i++){
     
   // Last i elements are already in place  
   for(var j = 0; j < ( res.length - i -1 ); j++){
       
     // Checking if the item at present iteration 
     // is greater than the next iteration
     if(res[j] > res[j+1]){
         
       // If the condition is true then swap them
       temp_na = na[j];
       na[j] = na[j + 1];
       na[j+1] = temp_na;
       
       temp_price = price[j];
       price[j] = price[j + 1];
       price[j+1] = temp_price;
       
       temp_res = res[j];
       res[j] = res[j + 1];
       res[j+1] = temp_res;
       
       temp_mem = mem[j];
       mem[j] = mem[j + 1];
       mem[j+1] = temp_mem;
       
       temp_cpu = cpu[j];
       cpu[j] = cpu[j + 1];
       cpu[j+1] = temp_cpu;
       
       temp_gpu = gpu[j];
       gpu[j] = gpu[j + 1];
       gpu[j+1] = temp_gpu;
       
       temp_storage = storage[j];
       storage[j] = storage[j + 1];
       storage[j+1] = temp_storage;
     }
   }
  }
}
function sort_mem() {
  var temp_na;
  var temp_price;
  var temp_res; 
  var temp_mem;
  var temp_cpu;
  var temp_gpu;
  var temp_storage;

  for(var i = 0; i < mem.length; i++){
     
   // Last i elements are already in place  
   for(var j = 0; j < ( mem.length - i -1 ); j++){
       
     // Checking if the item at present iteration 
     // is greater than the next iteration
     if(mem[j] > mem[j+1]){
         
       // If the condition is true then swap them
       temp_na = na[j];
       na[j] = na[j + 1];
       na[j+1] = temp_na;
       
       temp_price = price[j];
       price[j] = price[j + 1];
       price[j+1] = temp_price;
       
       temp_res = res[j];
       res[j] = res[j + 1];
       res[j+1] = temp_res;
       
       temp_mem = mem[j];
       mem[j] = mem[j + 1];
       mem[j+1] = temp_mem;
       
       temp_cpu = cpu[j];
       cpu[j] = cpu[j + 1];
       cpu[j+1] = temp_cpu;
       
       temp_gpu = gpu[j];
       gpu[j] = gpu[j + 1];
       gpu[j+1] = temp_gpu;
       
       temp_storage = storage[j];
       storage[j] = storage[j + 1];
       storage[j+1] = temp_storage;
     }
   }
  }
}
function sort_cpu() {
  var temp_na;
  var temp_price;
  var temp_res; 
  var temp_mem;
  var temp_cpu;
  var temp_gpu;
  var temp_storage;

  for(var i = 0; i < cpu.length; i++){
     
   // Last i elements are already in place  
   for(var j = 0; j < ( cpu.length - i -1 ); j++){
       
     // Checking if the item at present iteration 
     // is greater than the next iteration
     if(cpu[j] > cpu[j+1]){
         
       // If the condition is true then swap them
       temp_na = na[j];
       na[j] = na[j + 1];
       na[j+1] = temp_na;
       
       temp_price = price[j];
       price[j] = price[j + 1];
       price[j+1] = temp_price;
       
       temp_res = res[j];
       res[j] = res[j + 1];
       res[j+1] = temp_res;
       
       temp_mem = mem[j];
       mem[j] = mem[j + 1];
       mem[j+1] = temp_mem;
       
       temp_cpu = cpu[j];
       cpu[j] = cpu[j + 1];
       cpu[j+1] = temp_cpu;
       
       temp_gpu = gpu[j];
       gpu[j] = gpu[j + 1];
       gpu[j+1] = temp_gpu;
       
       temp_storage = storage[j];
       storage[j] = storage[j + 1];
       storage[j+1] = temp_storage;
     }
   }
  }
}
function sort_gpu() {
  var temp_na;
  var temp_price;
  var temp_res; 
  var temp_mem;
  var temp_cpu;
  var temp_gpu;
  var temp_storage;

  for(var i = 0; i < gpu.length; i++){
     
   // Last i elements are already in place  
   for(var j = 0; j < ( gpu.length - i -1 ); j++){
       
     // Checking if the item at present iteration 
     // is greater than the next iteration
     if(gpu[j] > gpu[j+1]){
         
       // If the condition is true then swap them
       temp_na = na[j];
       na[j] = na[j + 1];
       na[j+1] = temp_na;
       
       temp_price = price[j];
       price[j] = price[j + 1];
       price[j+1] = temp_price;
       
       temp_res = res[j];
       res[j] = res[j + 1];
       res[j+1] = temp_res;
       
       temp_mem = mem[j];
       mem[j] = mem[j + 1];
       mem[j+1] = temp_mem;
       
       temp_cpu = cpu[j];
       cpu[j] = cpu[j + 1];
       cpu[j+1] = temp_cpu;
       
       temp_gpu = gpu[j];
       gpu[j] = gpu[j + 1];
       gpu[j+1] = temp_gpu;
       
       temp_storage = storage[j];
       storage[j] = storage[j + 1];
       storage[j+1] = temp_storage;
     }
   }
  }
}
function sort_storage() {
  var temp_na;
  var temp_price;
  var temp_res; 
  var temp_mem;
  var temp_cpu;
  var temp_gpu;
  var temp_storage;

  for(var i = 0; i < storage.length; i++){
     
   // Last i elements are already in place  
   for(var j = 0; j < ( storage.length - i -1 ); j++){
       
     // Checking if the item at present iteration 
     // is greater than the next iteration
     if(storage[j] > storage[j+1]){
         
       // If the condition is true then swap them
       temp_na = na[j];
       na[j] = na[j + 1];
       na[j+1] = temp_na;
       
       temp_price = price[j];
       price[j] = price[j + 1];
       price[j+1] = temp_price;
       
       temp_res = res[j];
       res[j] = res[j + 1];
       res[j+1] = temp_res;
       
       temp_mem = mem[j];
       mem[j] = mem[j + 1];
       mem[j+1] = temp_mem;
       
       temp_cpu = cpu[j];
       cpu[j] = cpu[j + 1];
       cpu[j+1] = temp_cpu;
       
       temp_gpu = gpu[j];
       gpu[j] = gpu[j + 1];
       gpu[j+1] = temp_gpu;
       
       temp_storage = storage[j];
       storage[j] = storage[j + 1];
       storage[j+1] = temp_storage;
     }
   }
  }
}
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
//Low-Find
onEvent("Find_Low", "change", function( ) {
var low_dropdown = getProperty("Find_Low","value");
  //1
  if(low_dropdown == "Lowest Tier"){
  sort_price(true);
  
  setText("Low_text_area", "The Lowest Tier Computer that can be purchased is: The " + na[0] + " for $"+ price[0] 
  + "\n" + " The Specs are: " + "\n" + "1. Resolution: "+ res[0]+ "\n" +"2. Memory: "+ mem[0]+ "\n" +"3. CPU: "+ 
  cpu[0]+ "\n" +"4. GPU: "+ gpu[0]+ "\n" +"5. Storage "+ storage[0]);
  
  }
  //2
  if(low_dropdown == "Find"){
  setText("Low_text_area","PLEASE SELECT A CHOICE!");
  }
});
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
//Mid-Find
onEvent("Find_Mid", "change", function( ) {
var mid_dropdown = getProperty("Find_Mid","value");
  //1
  if(mid_dropdown == "Medium-Price"){
sort_price(true);

  setText("Mid_text_area", "The Medium Tier Computer that can be purchased is: The " + na[na.length-125] + 
  " for $"+ price[price.length-125] + "\n" + " The Specs are: " + "\n" + "1. Resolution: "+ res[res.length-125]+
  "\n" +"2. Memory: "+ mem[mem.length-125]+ "\n" +"3. CPU: "+ cpu[cpu.length-125]+ "\n" +"4. GPU: "+ 
  gpu[gpu.length-125]+ "\n" +"5. Storage "+ storage[storage.length-125]);
  
  }
  //2
  if(mid_dropdown == "Find"){
  setText("Mid_text_area","PLEASE SELECT A CHOICE!");
  }
});
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
//Ultimate-Find
onEvent("Find_Ultimate", "change", function( ) {
var ultimate_dropdown = getProperty("Find_Ultimate","value");
  //1
  if(ultimate_dropdown == "Maximum-Price"){
 sort_price(true);
 
  setText("Ultimate_text_area","The Ultimate Tier Computer that can be purchased is: The " + na[na.length-1] + 
  " for $"+ price[price.length-1] + "\n" + " The Specs are: " + "\n" + "1. Resolution: "+ res[res.length-1]+ 
  "\n" +"2. Memory: "+ mem[mem.length-1]+ "\n" +"3. CPU: "+ cpu[cpu.length-1]+ "\n" +"4. GPU: "+ 
  gpu[gpu.length-1]+ "\n" +"5. Storage "+ storage[storage.length-1]);
  
  }
  //2
  if(ultimate_dropdown == "Find"){
  setText("Ultimate_text_area","PLEASE SELECT A CHOICE!");
  }
});
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*
Credits:
Doc Oliver created a Scalper to pull data from a popular website,"PCPartPicker".
The total amount of items scalped is Part count: 45,424 ...as of July 11, 2021
The only data set Used was 'Laptops'
https://github.com/docyx/pc-part-dataset
*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
//Json to CSV converter
//https://data.page/json/csv
//Data Pulled:

/*

                      Table/Topic:  *Laptop's*

Columns: 1-8

1. Name
2. Price
3. Screen Size
4. Resolution
5. Memory
6. CPU
7. Storage
8. GPU

*/

/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
//Button Screen to Screen Operations
//Home to Low
onEvent("Low", "click", function( ) {
setScreen("Low-Range");
});
//Low to Home
onEvent("lowHome", "click", function( ) {
setScreen("homeScreen");
});
//Home to Mid
onEvent("Mid", "click", function( ) {
setScreen("Mid-Range");
});
//Mid to Home
onEvent("midHome", "click", function( ) {
setScreen("homeScreen");
});
//Home to Ultimate
onEvent("Ultimate", "click", function( ) {
setScreen("Ultimate-Range");
});
//Ultimate to Home
onEvent("ultimateHome", "click", function( ) {
setScreen("homeScreen");
});
/*----------------------------------------------------------------------------------*/
/*----------------------------------------------------------------------------------*/
