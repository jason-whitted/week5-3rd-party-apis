# Bootstrap Grid System

> Use our powerful mobile-first flexbox grid to build layouts of all shapes and sizes thanks to a twelve
> column system, five default responsive tiers, Sass variables and mixins, and dozens of predefined classes.

## Twelve Column System

![](https://www.c-sharpcorner.com/article/bootstrap-grid-system/Images/1.png)

## Five Default Responsive Tiers
Pre-defined, named tipping points.

| Name | Size              |
|------|-------------------|
| `xs` | <576px (mobile)   |
| `sm` | ≥576px            |
| `md` | ≥768px            |
| `lg` | ≥992px            |
| `xl` | ≥1200px (desktop) |

## Containers, Rows, and Columns
Your page should have one `container`.

A `row` can contain any number of **columns**.  The grid system uses flexbox so the content will wrap seemlessly, but you can use more than row to ensure that your content is properly divided.

Columns are specified using:
- `col-#` - where `#` is the number of columns to span (1 to 12)
- `col-??-#` - where `??` is one of the pre-defined tipping points
