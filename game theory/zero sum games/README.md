# Игра с нулевой суммой: оптимизация стратегий с использованием линейного программирования

Этот проект реализует решение задачи теории игр для **игры с нулевой суммой** с использованием Python и библиотек `numpy`, `scipy` и `seaborn`. В задачах такого типа выигрыш одного игрока является проигрышем другого, и оптимальные стратегии определяются с помощью **минимаксного подхода**.

## Описание кода

### Основные компоненты
1. **Генерация матрицы выплат**: 
    Матрица выплат (`payoff_matrix`) задаёт выигрыш или проигрыш игрока 1 при разных сочетаниях стратегий обоих игроков. В данном примере создаётся случайная матрица выплат размером 4x4 для симуляции различных игровых ситуаций.

2. **Функция `solve_zero_sum_game`**:
    Главная функция, которая решает игру с нулевой суммой, используя методы линейного программирования для нахождения оптимальных стратегий обоих игроков и значения игры:
   
   - **Шаги для игрока 1**: 
     - Формулируется задача линейного программирования для игрока 1, минимизирующего свой наибольший возможный проигрыш (или максимизирующего минимальный выигрыш).
     - Решение оптимизирует вероятности стратегий игрока 1, которые минимизируют его риск в наихудшем случае.

   - **Шаги для игрока 2**: 
     - Задача линейного программирования для игрока 2 направлена на минимизацию максимального выигрыша игрока 1.
     - Если решение для игрока 2 невозможно, вероятность стратегий игрока 2 устанавливается на нулевой вектор, и выводится предупреждающее сообщение.

3. **Визуализация результатов**:
    - **Матрица выплат**: Визуализируется с помощью `seaborn.heatmap`, чтобы наглядно показать зависимости выигрышей и проигрышей при различных комбинациях стратегий игроков.
    - **Вероятности стратегий**: Оптимальные вероятности стратегий для каждого игрока отображаются на гистограмме (`seaborn.barplot`), чтобы продемонстрировать распределение стратегий для обоих игроков.

### Структура кода

```python
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
from scipy.optimize import linprog

# Генерация случайной матрицы выплат
np.random.seed(42)
payoff_matrix = np.random.randint(-10, 10, (4, 4))

# Функция для нахождения оптимальных стратегий
def solve_zero_sum_game(payoff_matrix):
    # ... [полный код функции]
    return probabilities_1, probabilities_2, game_value

# Запуск и вывод результатов
probabilities_1, probabilities_2, game_value = solve_zero_sum_game(payoff_matrix)
print("Оптимальные вероятности стратегий:", probabilities_1, probabilities_2)
print("Значение игры:", game_value)

# Визуализация
fig, ax = plt.subplots(1, 2, figsize=(14, 6))
sns.heatmap(payoff_matrix, annot=True, fmt="d", cmap="coolwarm", ax=ax[0])
sns.barplot(x="Стратегии", y="Вероятности", hue="Игрок", data=strategies_df, palette="viridis", ax=ax[1])
plt.tight_layout()
plt.show()

```

## Примечания

Проверка допустимости решения : если задача для одного из игроков не имеет решения, код выдает предупреждение о том, что он делает устойчивые ошибки, и позволяет проанализировать даже сложные случаи.
Методlinprog из scipy.optimize: Используется для минимизации или максимизации выигрыша в условиях линейных ограничений. Это позволяет решать задачи по оптимизации даже при большой размерности стратегии.


## Зависимости


- numpy: для работы с матрицами и массивами.
- scipy: для решения задач линейного программирования.
- seabornи matplotlib: для визуализации данных и оптимизации результатов.