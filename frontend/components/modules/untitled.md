# Accordion

## Usage

1. Import the Accordion module in the page’s JavaScript file.

```javascript
import Accordion from './modules/accordion';
```

2. Layout your markup like this:

```markup
<div data-accordion="example">
    <div data-accordion-block>
        <div data-accordion-trigger>Trigger 1</div>
        <div data-accordion-content>
            <div>
                <div>Content</div>
                <div>Content</div>
            </div>
        </div>
    </div>
    <div data-accordion-block>
        <div data-accordion-trigger>Trigger 2</div>
        <div data-accordion-content>
            <div>
                <div>Content</div>
                <div>Content</div>
                <div>Content</div>
            </div>
        </div>
    </div>
    <div data-accordion-block>
        <div data-accordion-trigger>Trigger 3</div>
        <div data-accordion-content>
            <div>
                <div>Content</div>
            </div>
        </div>
    </div>
</div>
```

3. Create an Accordion instance with a reference to a DOM element.

```javascript
new Accordion(accordionId, [options]);
```

## Properties <a id="AccordionModule-AdditionalOptions"></a>

| Option | Type | Default value | Description |
| :--- | :--- | :--- | :--- |
| collapseOthers | boolean | false | Boolean for whether or not to collapse all other panels when one panel is open |
| maxWorkingWidth | number | false | Maximum width at which the Accordion Module working |

## Methods

| Option | Type | Description |
| :--- | :--- | :--- |
| onClose | function | Callback on close event |
| onOpen | function | Callback on open event |

## Example <a id="AccordionModule-Example"></a>

```javascript
new Accordion('example', {
  collapseOthers: true,
  maxWorkingWidth: 1200,
  onOpen: function() {
    console.log('trigger open event');
  };
});
```

