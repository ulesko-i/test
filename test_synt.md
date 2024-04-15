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

Таблица с `border=0` и объединенными ячейками, содержимое которых выровнено по центру.

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


## HTML-3

Таблица с проверкой визуализации объединения ячеек.

<table border=0>
    <tbody>
        <tr>
            <td rowspan=5>
                <h2>Заголовок блока 1</h2>
            </td>
            <td>
                <h3>Заголовок текста 1-1</h3>
                <em>Курсив под заголовком 1-1</em><br><br>
                Абзац с обычным текстом. Абзац с обычным текстом. Абзац с обычным текстом. Абзац с обычным текстом.<br>
                Подводка к <b>списку</b>:
                <li>
                    Первый элемент списка.
                </li>
                <li>
                    Второй элемент списка.
                </li>
                <li>
                    Третий элемент списка с <a href="https://htmlbook.ru/html/a">гиперссылкой</a>.
                </li>
                Новый абзац с обычным текстом.
            </td>
        </tr>
        <tr>
            <td>
                <h3>Заголовок текста 1-2</h3>
                <em>Курсив под заголовком 1-2</em><br><br>
                Абзац с обычным текстом. Абзац с обычным текстом. Абзац с обычным текстом. Абзац с обычным текстом.<br>
                Подводка к <b>списку</b>:
                <li>
                    Первый элемент списка.
                </li>
                <li>
                    Второй элемент списка.
                </li>
                <li>
                    Третий элемент списка с <a href="https://htmlbook.ru/html/a">гиперссылкой</a>.
                </li>
                Новый абзац с обычным текстом.
            </td>        </tr>
        <tr>
            <td>text1-3</td>
        </tr>
        <tr>
            <td>text1-4</td>
        </tr>
        <tr>
            <td>text1-5</td>
        </tr>
        <tr>
            <td rowspan=2>
                <h2>Заголовок блока 2</h2>
            </td>
            <td>text2-1</td>
        </tr>
        <tr>
            <td>text2-2</td>
        </tr>
        <tr>
            <td rowspan=2>XXXXX3</td>
            <td>text3-1</td>
        </tr>
        <tr>
            <td>text3-2</td>
        </tr>
        <tr>
            <td>XXXXX4</td>
            <td>text4-1</td>
        </tr>
    </tbody>
</table>