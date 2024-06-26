---
description: Calibration -> Lens Distortion
---

# Калибровка Lens Distortion

1. Убедитесь  что у вас указаны [**мин и макс для значений энкодеров.**](../nastroika-ustroistv/podklyuchenie-enkoderov-zoom-focus/)
2. Перейдите в раздел **Calibration -> Lens Distortion.** В разделе **Calibration** в поля **Chessboard width** и **Chessboard height** укажите количество клеток выбранной таблицы. В выпадающем списке **Mode**, укажите необходимый набор параметров кривизны. Важно! k3 поддерживается только в Unreal Engine, остальные ПО используют только k1, k2.

**Замечание**: Для получения большей глубины резкости, рекомендуем прикрыть диафрагму, а шахматную таблицу показывать с монитора ноутбука или большого планшета.

3. Установите зум и фокус на минимальное значение. Сделайте 6 снимков, путем нажатия на кнопку **Capture image.** Очередность снимков не имеет значения. Убедитесь что выбран верный **Mode** и нажмите на кнопку **Calibrate.**

**Важно!** Края таблицы не должны выходить за границу кадра. таблицу держите перпендикулярно оси камеры.

{% embed url="https://youtu.be/Jetsu0T3oRM" %}

4. В окне консоли отобразятся высчитанные значения с указанием размера ошибки при вычислениях - **Reprojection error** (полученное значение, означает размер ошибки в пикселях. Рекомендуем использовать значения укладывающиеся до Reprojection error : 1).&#x20;

**Замечание**: Обратите внимание на окно **Image list**. Система подсветит зелеными рамками фотографии которые распознала, а красными которые нет. Их следует удалить и сделать новые, затем нажать на Calibrate и сравнить размер ошибки. Если у вас была создана калибровка с большим значением **Reprojection error**, то ее следует удалить. Для этого прокрутить окно вниз и в разделе **Calibration date**, выберите необходимую калибровку и нажмите **Delete distortion**. Дисторсии с одинаковыми значениями фокуса и зума будут подсвечены красным в разделе **Calibration date**.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_НУЖНО ВИДЕО С ОШИБКОЙ И УДАЛЕНИЕМ ФОТО И ДИСТОРСИИ\_\_\_\_\_\_

5. Удалите фотографии в окне **Image list**, нажав кнопку **Clear images** под ним.

<figure><img src="../../.gitbook/assets/Lens distortion clear images.png" alt=""><figcaption></figcaption></figure>

6. Повторите шаг №3 для фокуса 0 и 1 на значениях зума 0, 0.25, 0.5, 1, если у вас fix zoom, то только 2 калибровки для фокуса 0 и 1. Для удобства рекомендуем ориентироваться на подсказку. В разделе **Calibration data** красным отмечены позиции на которых вам необходимо сделать калибровку, после создания калибровки, в графике точка соответсвующая данным поменяет цвет на зеленый.

<figure><img src="../../.gitbook/assets/Lens distortion. value zf.png" alt=""><figcaption></figcaption></figure>

7. По завершению калибровки в окне **Interpolation** выберите **Mode** -> **Spline** и нажмите **Set value**.  После этого вы можете перейти в [**графики**](../grafiki.md), нажав кнопку **Chart** и посмотреть как система догенирировала необходимые значения.

{% embed url="https://youtu.be/O5J5UAHGUeo" %}
