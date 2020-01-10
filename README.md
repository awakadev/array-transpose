# Array Transpose
```
      list: [
        {
          ping: 70,
          indicator: 'active',
          id: 1,
          name: 'Fidela1',
          group: 'Fidela',
          route: '165.9.197.163'
        },
        {
          ping: 55,
          indicator: 'intermediary',
          id: 2,
          name: 'Garrard',
          group: 'Fidela',
          route: '138.87.225.97'
        },
        {
          ping: 100,
          indicator: 'positive',
          id: 3,
          name: 'Clayborn1',
          group: 'Clayborn',
          route: '237.146.154.222'
        },
        {
          ping: 12,
          indicator: 'negative',
          id: 6,
          name: 'Elna',
          group: 'Clayborn',
          route: '53.209.210.199'
        },
        {
          ping: 0,
          indicator: 'positive',
          id: 8,
          name: 'Fidela2',
          group: 'Fidela',
          route: '219.29.191.217'
        },
        {
          ping: 68,
          indicator: 'active',
          id: 4,
          name: 'Reinaldos',
          group: 'Clayborn',
          route: '35.148.222.21'
        },
        {
          ping: 1143,
          indicator: 'intermediary',
          id: 5,
          name: 'Abigael',
          group: 'Richmond',
          route: '135.221.192.85'
        },
        {
          ping: 100,
          indicator: 'positive',
          id: 7,
          name: 'Lanna',
          group: 'Clayborn',
          route: '198.34.29.215'
        },
        {
          ping: 88,
          indicator: 'active',
          id: 9,
          name: 'Mamie',
          group: 'Richmond',
          route: '69.0.235.44'
        },
        {
          ping: 9,
          indicator: 'negative',
          id: 10,
          name: 'Saudra',
          group: 'Clayborn',
          route: '182.157.218.101'
        }
      ],
      keys: ['indicator', 'name', 'group', 'ping', 'route', 'id']
```
_____
```      
      const transpose = (items) => {
        return this.keys.map((key) => {
          return items.map((item) => {
            return item[key] || ''
          })
        })
      }
      return transpose(this.list)
```
