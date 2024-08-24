let items = [{ value: 1, day: '2021-09-11' },
  { value: 4, day: '2021-09-11' },
  { value: 5, day: '2021-09-11' },
  { value: 5, day: '2021-09-12' },
  { value: 3, day: '2021-09-12' },
  { value: 5, day: '2021-09-12' },
  { value: 1, day: '2021-09-13' }];
  
  items.reduce((acc, c) => (acc[c.day] ??= acc[c.day] =+ c.value  , acc), {});
