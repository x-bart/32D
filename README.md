# Тридцать два гнома

Поведеньческая модель гнома

# Основные объекты

## Мир

* 2D поле NxM клеток склеенное второид
* содержит:
  * Пустые клетки (Пещеры)
  * Клетки занятые породой (Думаю их можно копать)
  * Клетки с едой (Грибы)
  * Клетки с гномами (Своими и чужими)

## Гном

* Модель гнома имеет следующие праметры:
  * Положение в мире х, y
  * Энергия  0-100
  * Сытость  0-100
  * Здоровье 0-100
* Действия гнома
  * Отдых
  * Передвижение
  * Питание
  * Атака
  * *Копание?*
* Каждое действие гнома однимает **de** энергии, отдых восстанавливает **re** энергии и **rh** здоровья
* Каждый тик сытость гнома убывает на **ds**, если сытость гнома равна нулю начинает убывать здоровье на **dh**
* Съеденный гриб восстанавливает сытость на **mrs**, а здоровье на **mrh**

## Гриб

В мире всегда есть **М** грибов, как только один гриб съеден, в мире появляется новый в случайном месте
