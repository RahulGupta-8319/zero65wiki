## API Response Format:
```
{

  heads: [
    ...
    {
      key: 'id' | <string>,
      title: <string>,
      align: 'start' | 'center' | 'end',
      format: 'number' | 'number2d' | 'number3d' | 'percentage2d' | 'percentage4d' | 'currencyInr' | 'currencyInr2d',
      gradient: {
        min: Float,
        max: Float
      },
      hide: true | false
    },
    ...
  ],

  rows: [
    ...
    [ ... ],
    ...
  ],

  messages: {
    ...
    rowId: { headKey: <string> } 
    ...
  },

  refresh: seconds

}
```
