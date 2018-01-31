Документація базується на документ–генераторі [**Daux.io**](https://github.com/dauxio/daux.io).

## Інсталяція

Насамперед необхідно, щоб у вас був встановлена інтерпритатор мови програмування [PHP](https://php.net) версії не нижче 5.4 та його розширення [composer](https://getcomposer.org/). Далі зайдіть в папку `krogerc-ecomon-man-api`, та виконайте команду, після якої будуть встановлені всі необхідні додатки.

```
composer update
```

## Старт динамічної документації

Для старту документації, необхідно виконати

```
serve
```

Після чого можна зайти з браузера за адресою `http://<ваш хост>:8085/`

## Генерація статичної документації

Є можливість сгенерувати статичну HTML-документацію.

```
generate
```

Після виконання в директорії `static` буде розміщено корінь із всіма сторінками. Для браузінгу відкривайте сторінку `index.html` у браузеру.

## Підтримка

Якщо знайшли помилку або маєте пропозиції щодо покращення документації, то просимо вас повідомити:

- [GitHub issue](https://github.com/novakom-devel/krogerc-komgosp-man-bill/issues)
- на електрону пошту <a href="mailto:novakom.devel@gmail.com?subject=Krogerc ecomon issue">novakom.devel@gmail.com</a>
- завести заявку у [центрі звернень криворізького русерсного центру](https://krogerc.info/ua/komcentr/register/internal.html) тільки для зареєстрованих користувачів
