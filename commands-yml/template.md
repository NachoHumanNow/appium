[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
# {{name}}

{{short_description}}
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
## Example Usage

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
```java
{{#if example_usage.java}}
// Java
{{example_usage.java}}
{{else}}
// Not supported
{{/if}}
```

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
```python
{{#if example_usage.python}}
# Python
{{example_usage.python}}
{{else}}
# Not supported
{{/if}}
```

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
```javascript
{{#if example_usage.javascript_wdio}}
// Javascript
// webdriver.io example
{{example_usage.javascript_wdio}}
{{else}}
// Not supported
{{/if}}


[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
{{#if example_usage.javascript_wd}}
// wd example
{{example_usage.javascript_wd}}
{{else}}
// Not supported
{{/if}}
```

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
```ruby
{{#if example_usage.ruby}}
# Ruby
# ruby_lib example
{{example_usage.ruby}}
{{else}}
# Not supported
{{/if}}

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
{{#if example_usage.ruby_core}}
# ruby_lib_core example
{{example_usage.ruby_core}}
{{else}}
# Not supported
{{/if}}
```

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
```php
{{#if example_usage.php}}
# PHP
{{example_usage.php}}
{{else}}
// Not supported
{{/if}}
```

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
```csharp
{{#if example_usage.csharp}}
// C#
{{example_usage.csharp}}
{{else}}
// Not supported
{{/if}}
```

{{#if selector_strategies}}
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
## Selector Strategies
|Strategy|Description|
|--------|-----------|
{{#each selector_strategies}}
|{{this.name}}|{{this.description}}|
{{/each}}
{{/if}}

{{#if description}}
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})
## Description

{{description}}
{{/if}}

## Support
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})

### Appium Server
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})

|Platform|Driver|Platform Versions|Appium Version|Driver Version|
|--------|----------------|------|--------------|--------------|
{{#each driver_support.ios}}
| {{#if @first}}iOS{{/if}} | [{{capitalize @key}}](/docs/en/drivers/ios-{{@key}}.md) | {{versions this "platform" @key}} | {{versions this "appium" @key}} | {{versions this "driver" @key}} |
{{/each}}
{{#each driver_support.android}}
| {{#if @first}}Android{{/if}} | [{{capitalize @key}}](/docs/en/drivers/android-{{@key}}.md) | {{versions this "platform" @key}} | {{versions this "appium" @key}} | {{versions this "driver" @key}} |
{{/each}}
{{#each driver_support.mac}}
| {{#if @first}}Mac{{/if}} | [{{capitalize @key}}](/docs/en/drivers/{{@key}}.md) | {{versions this "platform" @key}} | {{versions this "appium" @key}} | {{versions this "driver" @key}} |
{{/each}}
{{#each driver_support.windows}}
| {{#if @first}}Windows{{/if}} | [{{capitalize @key}}](/docs/en/drivers/{{@key}}.md) | {{versions this "platform" @key}} | {{versions this "appium" @key}} | {{versions this "driver" @key}} |
{{/each}}

### Appium Clients
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})

|Language|Support|Documentation|
|--------|-------|-------------|
|[Java](https://github.com/appium/java-client/releases/latest)| {{versions client_support.java}} | {{client_url client_docs.java}} |
|[Python](https://github.com/appium/python-client/releases/latest)| {{versions client_support.python}} | {{client_url client_docs.python}} |
|[Javascript (WebdriverIO)](http://webdriver.io/index.html)| {{versions client_support.javascript_wdio}} | {{client_url client_docs.wdio}} |
|[Javascript (WD)](https://github.com/admc/wd/releases/latest)| {{versions client_support.javascript_wd}} | {{client_url client_docs.javascript_wd}} |
|[Ruby](https://github.com/appium/ruby_lib/releases/latest)| {{versions client_support.ruby}} | {{client_url client_docs.ruby}} |
|[PHP](https://github.com/appium/php-client/releases/latest)| {{versions client_support.php}} | {{client_url client_docs.php}} |
|[C#](https://github.com/appium/appium-dotnet-driver/releases/latest)| {{versions client_support.csharp}} | {{client_url client_docs.csharp}} |

## HTTP API Specifications

### Endpoint
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})

`{{uppercase endpoint.method}} {{endpoint.url}}`

### URL Parameters
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})

{{#if endpoint.url_parameters}}
|name|description|
|----|-----------|
{{#each endpoint.url_parameters}}
|{{this.name}}|{{this.description}}|
{{/each}}
{{else}}
None
{{/if}}

### JSON Parameters
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})

{{#if endpoint.json_parameters}}
|name|type|description|
|----|----|-----------|
{{#each endpoint.json_parameters}}
| {{{this.name}}} | `{{{this.type}}}` | {{{this.description}}} |
{{/each}}
{{else}}
None
{{/if}}

### Response
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})

{{#if endpoint.response}}
{{#if_eq endpoint.response.length 1}}
{{endpoint.response.0.description}} (`{{endpoint.response.0.type}}`)
{{else}}
|name|type|description|
|----|----|-----------|
{{#each endpoint.response}}
| {{this.name}} | `{{this.type}}` | {{this.description}} |
{{/each}}
{{/if_eq}}
{{else}}
null
{{/if}}

## See Also
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in {{ymlFileName}})

{{#if specifications.w3c}}
* [W3C Specification]({{spec_url specifications.w3c endpoint.url}})
{{/if}}
{{#if specifications.jsonwp}}
* [JSONWP Specification]({{spec_url specifications.jsonwp endpoint.url}})
{{/if}}
{{#each links}}
* [{{this.name}}]({{this.url}})
{{/each}}