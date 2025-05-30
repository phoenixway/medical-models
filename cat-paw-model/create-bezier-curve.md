---
up:
  - "[[cat-paw-model]]"
---
Точне моделювання шляху вени (Vena Cephalica)**

1. **Створення кривої Безьє:** Як і раніше, додайте криву (`Shift+A` -> `Curve` -> `Bezier`). Назвіть її "CephalicVein".
2. **Редагування шляху (Найважливіший етап!):**
    - Перейдіть в `Edit Mode` (`Tab`) для кривої.
    - **Уважно вивчіть ваші анатомічні схеми!** Vena cephalica зазвичай проходить по передньо-медіальній (краніомедіальній) поверхні передпліччя.
    - Починайте розміщувати контрольні точки кривої (`G`), екструдувати (`E`) та налаштовувати ручки (`G`, `R`, `S`), щоб крива **точно** повторювала шлях вени відносно ваших спрощених моделей кісток та позначених суглобів (ліктьового та зап'ястного). Зверніть увагу, як вена проходить через ліктьову ямку та вздовж передпліччя до зап'ястя. _Саме ця точність є ключовою для вашої мети._
3. **Додавання товщини вені:**
    - Перейдіть в `Object Data Properties` (зелена крива) -> `Geometry` -> `Bevel`.
    - Встановіть `Depth`, щоб надати вені реалістичної товщини.
    - Налаштуйте `Resolution` для гладкості.
    - Можна поставити `Fill Caps`.
4. **Припасування до поверхні (Shrinkwrap):**
    - Додайте модифікатор `Shrinkwrap` до об'єкта вени (`Modifier Properties` -> `Add Modifier` -> `Shrinkwrap`).
    - В якості `Target` вкажіть об'єкт(и), що представляють поверхню кінцівки (якщо ви об'єднали кістки в один об'єкт (`Ctrl+J`) - вкажіть його; якщо ні - можливо, доведеться застосувати до кожної кістки окремо або створити допоміжну "оболонку" кінцівки).
    - Налаштуйте `Offset`, щоб вена трохи виступала над поверхнею.

**Крок 3: Фіналізація та акценти**

1. **Перевірка:** Ще раз уважно порівняйте положення вени на вашій моделі з анатомічними схемами, особливо відносно ліктьового та зап'ястного суглобів.
2. **Матеріали:** Призначте простий матеріал для кісток (білий/сірий), інший - для вени (синій або червонуватий, хоча вени традиційно сині на схемах), і яскравий - для маркерів суглобів (якщо ви їх додали).
3. **Анотації (якщо потрібно):** Використовуйте інструмент `Annotate` (на панелі інструментів зліва `T`) для додавання текстових позначок прямо у 3D-вікні, вказуючи на "Ліктьовий суглоб", "Зап'ястний суглоб", "Vena Cephalica".

**Результат:** У вас має вийти спрощена 3D-модель частини кінцівки кота, де чітко видно розташування ліктьового та зап'ястного суглобів, а головне – максимально точно відтворений тривимірний шлях головної вени (Vena cephalica) відносно цих анатомічних орієнтирів. Пам'ятайте, що ключ до реалістичності в цьому завданні – не фотореалізм рендеру, а точність відтворення анатомічного шляху вени на основі достовірних джерел.