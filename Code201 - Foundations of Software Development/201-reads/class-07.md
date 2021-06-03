# Tables 

### To create a Table we use <Table>

1- Use <tr> to indicate table rows
2- Use <td> to indicate data into each row
3- use <th> for table headings
4- For long tables you can split the table into a <thead>, 
<tbody>, and <tfoot>.

# Functions, Objects, method 

## Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names. 

### 
var hotel ={
    name:'quay'
    rooms: '40'
    booked: '15'

    checkAvailabitly: function(){
        return this.room - this.booked
    }
}

- hotel is an object 
- name, rooms, booked is a key
- quay, 40, 15 is a value
- checkAvailability is a method

