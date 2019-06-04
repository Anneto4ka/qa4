// ДЗ4. Объекты. Ссылочный тип данных
// Задание сложное и будет разбираться на доп занятии, но кто сделает 🎖.

// Ваше имя и фамилия: Hanna Skoropadska


// 1. Создайте объект который описывает автомобиль. 
// Учитывайте не только харатеристики, но и владельца, регистрационные данные
// * историю техобслуживания
// * историю владения
// Для заданий * нужно использовать массив объектов

const car = {
  brand : 'Jaguar',
  model : 'F-Type',
  made : 2016,
  VIN : '6JF584367FT568798',
  color : 'white',
  registration : {
    licensePlate : 'JSK455',
    expiration : 'September 2020',
  },
  owner : {
    firstName : 'Joanna',
    lastName : 'Smith',
    driverLisence : 'Y35172S',
    address : {
      city : 'Walnut Creek',
      zip : '94596',
    },
  },
  previousOwners : [
    {
      firstName : 'Alex',
      lastName : 'Brown',
    }, 
    {
      firstName : 'Bill',
      lastName : 'Hower',
    },
  ],
  maintanceRecords : [
    {
      date : '25 Jan 2017' , mileage : 5000, description : 'Oil change',
    },
    {
      date : '23 Aug 2017' , mileage : 6623, description : 'Oil change, Tire Rotation',
    },
    {
      date : '08 Mar 2018' , mileage : 7345, description : 'Oil change, A/C Cleaning',
    },
  ],
};


// 2. Создайте объекты владельцев автомобилей
let owner1 = {
  firstName : 'Alex',
  lastName : 'Brown',
};
let owner2 = {
  firstName : 'Alex',
  lastName : 'Bouldin',
};
let owner3 = {
  firstName : 'Joanna',
  lastName : 'Smith',
};

// 3. В автомобиле можно использовать ссылку на владельца. 
// Сделайте из автомобиля ссылку на его вдадельца
//car.owner = owner3

const car1 = {
  make : 'Jaguar',
  model : 'xe',
  byear : 2017,
  color : 'red',
  registration : {
    licensePlate : 'JSK354',
    expiration : 'September 2020',
  },
  owner : owner3,
  previousOwners : [ owner1, owner2 ],
};

// 4. Обращаясь через автомобиль к владельцу, удалите у него произвольное свойство 

delete (car.previousOwners);
delete (car1.owner.firstName);

console.log(car, car1);

// 5. Обращаясь через автомобиль к владельцу, добавьте новое свойство вдадельцу
 
//car.owner.address.city = 'Los Gatos'; changing existing properties
//car.owner.address.zip = '95030'; 

car.owner.address.state = 'CA'; // add new property


// 6. Проверьте что все сделано правильно и выведите результат в консоль
  
console.log(car.owner);

// 7. Покажите пример как сделать копию объекта

let copyCar = {}
Object.assign(copyCar, car1);

console.log('!!!!!!!!!!!!!!!');
console.log(copyCar);



// 8. Докажите, что вы сделали копию, а не скопировалии ссылку на один и тотже объект

car1.color = 'black';   //if I change color of car1 to black, in copyCar it should stay the same - red .
console.log(copyCar.color);
