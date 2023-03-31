Практика 0
@startuml
left to right direction
actor клиент
actor Ozon
rectangle Постомат {
клиент -- (Получить товар)
(Проверка номена заказа)
(Проверка наличия заявки на возврат)
клиент -- (Возврат)
(Получить товар) .> (Проверка номена заказа) : include
(Возврат) .> (Проверка наличия заявки на возврат) : include
Ozon -- (Проверка работоспособности)
}
@enduml

<img width="473" alt="Снимок экрана 2023-03-30 в 20 49 45" src="https://user-images.githubusercontent.com/91331145/229065723-0aed34e4-5812-42ec-bab0-8d8235ded0b2.png">
