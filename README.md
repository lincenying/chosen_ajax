# chosen_ajax
chosen ajax插件

```
$("#exp").ajaxChosen({
    type: 'GET',
    url: 'https://api.github.com/user/10840991/starred?page=1',
    dataType: 'json'
}, function(json) {
    var results = [];
    $.each(json, function(i, val) {
        results.push({
            id: val.id,
            name: val.name
        });
    });
    return results;
});
```
