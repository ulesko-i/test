# Проверка корректности отображения синтаксиса

## Тестирование HTML-таблицы

<table class="resume">
    <thead>
        <tr>
            <th>Заголовок 1</th>
            <th>Заголовок 2</th>
            <th>Заголовок 3</th>
        </tr>
    </thead>
	<tbody>
		<tr>
			<td>текст 1</td>
			<td>текст 2</td>
			<td>текст 3</td>
		</tr>
		<tr>
			<td>123</td>
			<td>234</td>
			<td>345</td>
		</tr>
		<tr>
			<td>123</td>
			<td>234</td>
			<td>
            Тестирование поддержки синтаксиса Markdown внутри ячейки:
            - список
            - список
            Список завершен.
            </td>
		</tr>
	</tbody>
</table>

## Тестирование MD-таблицы

| Заголовок 1 | Заголовок 2 |
| ----------- | ----------- |
| Текст внутри первого столбца | Текст во втором столбце |
|                              | Многострочный?            |


## HTML-2

Таблица с `border=0` и объядиненными ячейками, содержимое которых выровнено по центру.

<table border=0>
    <thead>
        <tr>
            <th>Column 1</th>
            <th>Column 2</th>
            <th>Column 3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=4 align="center"><h3>Заголовок уровня 3</h3>Обычный текст, после которого идет список:<li>первый элемент</li><li>второй элемент</li></td>
            <td rowspan=2 align="center">R2 Text A</td>
            <td align="center">R3 Text A</td>
        </tr>
        <tr>
            <td align="center">R3 Text B</td>
        </tr>
        <tr>
            <td rowspan=2 align="center">R2 Text B</td>
            <td align="center">R3 Text C</td>
        </tr>
        <tr>
            <td align="center">R3 Text D</td>
        </tr>
    </tbody>
</table>