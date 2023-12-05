## API Response Format:
```
{

  heads: [
    ...
    {
      key: 'id' | <string>,
      title: <string>,
      align: 'start' | 'center' | 'end',
      format: <string>,
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
   rowId: { headKey: <string> } 
  }

}
```
