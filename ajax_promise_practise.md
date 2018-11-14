#### Создайте html файл с формой где будут:

1) 4 инпута: name, lastName, phone и agree checkbox для подтверждения регистрации <br>
2) кнопка `Save User`

Обязательно:

1) Для каждого input обавьте уникальный id && name  <br>
2) Добавьте валидацию для инпутов (required for all, phone should match pattern: 000-000-00-00)

#### Создайте класс `People`, в котором будет прописана дальнейшая логика:

1. При нажатии на кнопку `Save User` мы собираем все значение с input, записываем в экземпляр класса Person (создайте этот класс перед class People):
```
{
    id: [number_of_user],
    name: "Vasya",
    lastName: "Koskin",
    phone: "380905675453",
    agree: true
};
```
и сохраняем через method=`PUT` `url=/people` если это новый Юзер или через `POST` если такой уже есть (сервер в ответ на PUT вернет вам что юзер уже есть и вам нужно будет сделать еще один запрос POST) но пока бэкенд условный, страница не должна презагружаться
2. В нем будет метод для вывода всего списка юзеров что у вас есть `method=GET` `url=/people`
3. Метод для вывода списка всех пользователей которые есть (список берем из пункта 2)
4. При добавлении пользователя через форму в вашем списке из 3 пунка должен появляться новый юзер в конец списка
5. Добавьте в списке для каждого элемента крестик справа, при нажатии на который юзер будет удаляться из DOM и на бэке (через запрос DELETE /people)

## Server to use for this purpose

Use this repo https://github.com/OlegPalchyk/testNodeServer clone it and follow the instructions. Than after starting server ($npm run dev) you will be able to send requests to this server on the URL='http://localhost:5000' + '/people' or other routes

### Sample code:

```

class Person {
  constructor ({ name, lastName, phone, agree }) {
    ... some code
  }

  getDOMElementCreated () {
    ... some code
  }

  insertIn (parent) {
    ... some code
  }
}



class PersonAPI {
  constructor({ URL }) {
    this.URL = URL;
  }

  getPersonsList () {
    return new Promise((resolve, reject) => {
      let xhr = new XMLHttpRequest();

      ...some code
    })
  }
  
  deletePersonById (id) { ... some code }
  
  addNewPersonById (id) { ... some code }
}
```
