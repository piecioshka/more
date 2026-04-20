# more

🛠 Truncate content in table cells.

## Preview 🎉

- <https://codepen.io/piecioshka/pen/GqZydL>
- <https://piecioshka.github.io/more/>

## Motivation

More about that tool (in Polish): <https://piecioshka.pl/blog/2014/01/30/narzedzia-swiata-more-js.html>

## Example

1. Before use:

    ![normal](https://piecioshka.pl/assets/images/posts/more-js/more-js-normal.png)

2. After use or after the 'less' link is clicked:

    ![collapse](https://piecioshka.pl/assets/images/posts/more-js/more-js-collapse.png)

3. After use and click the 'more' link:

    ![expand](https://piecioshka.pl/assets/images/posts/more-js/more-js-expand.png )

## Usage

Gigantic table in HTML:

```html
<table id="my_table" class="table table-striped table-bordered">
    <thead>
        <tr>
            <th>Column #1</th>
            <th>Column #2</th>
            <th>Column #3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque ac porttitor purus, vehicula varius metus. Suspendisse et pulvinar nulla. Pellentesque faucibus tristique risus sit amet eleifend. Proin augue elit, laoreet vestibulum mauris vitae, gravida consequat felis.</td>
            <td>Lorem ipsum dolor sit amet.</td>
            <td>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque ac porttitor purus, vehicula varius metus.</td>
        </tr>
        <tr>
            <td>Lorem ipsum dolor sit amet.</td>
            <td>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque ac porttitor purus, vehicula varius metus. Suspendisse et pulvinar nulla. Pellentesque faucibus tristique risus sit amet eleifend. Proin augue elit, laoreet vestibulum mauris vitae, gravida consequat felis.</td>
            <td>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque ac porttitor purus, vehicula varius metus.</td>
        </tr>
        <tr>
            <td>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque ac porttitor purus, vehicula varius metus. Suspendisse et pulvinar nulla. Pellentesque faucibus tristique risus sit amet eleifend. Proin augue elit, laoreet vestibulum mauris vitae, gravida consequat felis.</td>
            <td>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque ac porttitor purus, vehicula varius metus.</td>
            <td>Lorem ipsum dolor sit amet.</td>
        </tr>
    </tbody>
</table>
```

This line is responsible for the effect of truncating cell content.

```javascript
new More({
    selector: 'table#my_table',
    limit: 20 // limit cell content to 20 chars
});
```

## License

[The MIT License](https://piecioshka.mit-license.org) @ 2014
