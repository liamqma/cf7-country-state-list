## This is the fork from https://github.com/guardadoe/cf7-country-state-list

The reason is because I need the country code instead of country name. So now the country select has country code as option value. See below;

```HTML
<select onchange="printState('state',this.value);" id="country" name="country">
    <option value="AF">Afghanistan</option>
    <option value="AL">Albania</option>
    ...
</select>
```