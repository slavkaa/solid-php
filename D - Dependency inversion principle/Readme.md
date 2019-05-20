# Dependency inversion principle
_Принцип інверсії залежностей_

По підрічнику: 
 Модулі вищого рівня не повинні залежати від модулів нижчого рівня. Обидва типи модулів повинні залежати від абстракцій.
 Абстракції не повинні залежати від деталей реалізації. Деталі реалізації повинні залежати від абстракцій.
 
Людською мовою:
 Ми не остворюємо об'єекти в середині інших об'єктів. Для цього використовуються спеціаньні класси - фабрики.
 Ми конфігуруємо залежності між об'єктами, передаючі одні об'єкти у інші.
 Ми спираємось на відповідніст об'єта інтерфейсу, а не на приналежність до певного классу, коли передаємо
 один об'єкт у інший.
 
Прикладом реалізації цього приницпу є код класу Auth з папки "S - single responsibility / 1".
Там ми у конструкторі передаємо об'єкт, який чмплементує інтерфейс iLogger. Це дозволяє легко, на льоту міняти
 спосіб логування в залежності від наших потреб.
 