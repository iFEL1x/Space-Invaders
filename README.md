# <p align="center"> Space-Invaders</p>

<div align="Center">
    <img src = https://github.com/iFEL1x/iFEL1x/blob/main/Resources/Screenshots/Screen(Space-Invaders)(0).png width="600">
</div>

## Описание проекта

Данный проект является изучением статьи 
***"How to Make a Game Like Space Invaders"*** на сайте сообщества [www.kodeco.com](https://www.kodeco.com/)

Проект собран в Unity3D с использованием языка программирование C# и принципов ООП

___
## Скачивание и установка
Для того что бы запустить проект на своем ПК

* [Скачайте](https://unity3d.com/ru/get-unity/download) и [установите](https://docs.unity3d.com/2018.2/Documentation/Manual/InstallingUnity.html) Unity3D последней версии с официального сайта.
* Скачайте проект по [ссылке](https://github.com/iFEL1x/) или с текущей странице "Code\Download ZIP".
    + Распакуйте архив на своем ПК.
* Запустите Unity3D
    + Рядом с кнопкой "Open" нажмите на стрелочку :arrow_down_small:, в открывшимся списке выберете "Add project from disk"
    + Выберете путь распаковки проекта, нажмите "Add Project"

___
## В данном проекте применяется
* Массивы, циклы.
* Построение всего проекта максимально подводилось под ООП.

*Демонсрация кода:*

```C#
    private void MoveInvaders(float x, float y)
        {
            for(int i = 0; i < rowCount; i++)
            {
                for(int j = 0; j <columnCount; j++)
                {
                    invaders[i, j].Translate(x, y, 0);
                }
            }
        }

        private void ChangeDirection()
        {
            isMovingRight = !isMovingRight;
            MoveInvaders(0, -ySpacing);

            currentY -= ySpacing;
            if (currentY < minY)
                GameManager.Instance.TriggerGameOver();
        }
```

**Основная задача проекта** - Изучение возможностей Unity3D и языка программирования С# и принципов ООП.

*Демонстрация финальной части игрового процесса:*

![Space-Invaders](https://github.com/iFEL1x/iFEL1x/blob/main/Resources/Image/Gif/mp4%20to%20GIT(Space-Invaders).gif)
