Цель:

Создание интерфейса, который создаёт объект. При этом, выбор того, экземпляр какого класса создавать

остаётся за классами, которые имплементируют данный интерфейс.

Для чего используется:

Для делигирования полномочий создания экземпляров, другому классу.

Описание работы :

Нам нужно предоставить определенного продавца клиенту. Но чтобы каждый раз не создавать новый обьект самостоятельно , эту функцию мы предоставлям классам ,которые наслудуются от интерфейса SellerFactory,в котором есть реализован только один метод createSeller(). И уже при помощи метода createSellerBySpeciality(String speciality)

возвращается FoodSeller/HouseHoldSeller в зависимости от строки. Дальше мы создаем новый обьект класса ,который наследовался из Seller. Он создается при помощи метода createSeller(). Дальше вызывается метод sellGoods(), который переопределен для каждого класса.

![2020-02-25 (1)](https://user-images.githubusercontent.com/49583366/75205118-5cab7580-578c-11ea-89ed-5cdc6bf6ce0f.png)

![2020-02-25](https://user-images.githubusercontent.com/49583366/75205209-9bd9c680-578c-11ea-80ac-9180f9c239cf.png)

