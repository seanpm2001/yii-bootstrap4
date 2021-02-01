## Class Yiisoft\Yii\Bootstrap4\Progress
Renders a [bootstrap Progress bar component](https://getbootstrap.com/docs/4.5/components/progress/).

### Usage

```php
declare(strict_types=1);

use Yiisoft\Yii\Bootstrap4\Progress;

// default with label
echo Progress::widget()
    ->percent('60')
    ->label(test);
// styled
echo Progress::widget()
    ->bars([
        ['percent' => '65', 'options' => ['class' => 'bg-danger']]
    ]);
// striped
echo Progress::widget()
    ->bars([
        ['percent' => '70', 'options' => ['class' => 'bg-warning progress-bar-striped']]
    ]);
// striped animated
echo Progress::widget()
    ->percent('70')
    ->options(['class' => 'bg-success progress-bar-animated progress-bar-striped']);
// stacked bars
echo Progress::widget()
    ->bars([
        ['percent' => '30', 'options' => ['class' => 'bg-danger']],
        ['percent' => '30', 'label' => 'test', 'options' => ['class' => 'bg-success']],
        ['percent' => '35', 'options' => ['class' => 'bg-warning']],
    ]);
```
