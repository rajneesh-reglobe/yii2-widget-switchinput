yii2-widget-switch
==================

The SwitchInput widget turns checkboxes and radio buttons into toggle switches. The plugin is a wrapper for the [Bootstrap Switch Plugin](http://www.bootstrap-switch.org) and is specially styled for Bootstrap 3.

> NOTE: This extension is a sub repo split of [yii2-widgets](https://github.com/kartik-v/yii2-widgets). The split has been done since 08-Nov-2014 to allow developers to install this specific widget in isolation if needed. One can also use the extension the previous way with the whole suite of [yii2-widgets](http://demos.krajee.com/widgets).

## Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/). Check the [composer.json](https://github.com/kartik-v/yii2-widget-switch/blob/master/composer.json) for this extension's requirements and dependencies. Read this [web tip /wiki](http://webtips.krajee.com/setting-composer-minimum-stability-application/) on setting the `minimum-stability` settings for your application's composer.json.

To install, either run

```
$ php composer.phar require kartik-v/yii2-widget-switch "*"
```

or add

```
"kartik-v/yii2-widget-switch": "*"
```

to the ```require``` section of your `composer.json` file.

## Latest Release

> NOTE: The latest version of the module is v1.0.0 released on 08-Nov-2014. Refer the [CHANGE LOG](https://github.com/kartik-v/yii2-widget-switch/blob/master/CHANGE.md) for details.

## Demo

You can refer detailed [documentation and demos](http://demos.krajee.com/widget-details/switchinput) on usage of the extension.

## Usage

```php
use kartik\switch\SwitchInput;

// Usage with ActiveForm and model
echo $form->field($model, 'status')->widget(SwitchInput::classname(), [
    'type' => SwitchInput::CHECKBOX
]);


// With model & without ActiveForm
echo SwitchInput::widget([
    'name' => 'status_1',
    'type' => SwitchInput::RADIO
]);
```

## License

**yii2-widget-switch** is released under the BSD 3-Clause License. See the bundled `LICENSE.md` for details.