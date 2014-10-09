### This is the fork from https://github.com/guardadoe/cf7-country-state-list

The reason is that I need the country code instead of country name. The select box has country code as option value. See below;

```HTML
<select onchange="printState('state',this.value);" id="country" name="country">
    <option value="AF">Afghanistan</option>
    <option value="AL">Albania</option>
    ...
</select>
```

Feel free to fork it or send pull request if there is any mistake.
