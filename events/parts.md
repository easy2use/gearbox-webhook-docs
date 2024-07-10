# Part Webhook

## part.created event

```rb
{
  id: 1,
  part_number: 'ABC123',
  alternate_part_number: 'DAF321',
  description: 'Oil Filter',
  supplier: [
    {
      name: 'Repco',
      code: 'REP123'
    }
  ],
  each: 10.10,
  reorder: 10,
  stock_level: 20,
  each_type: 'ea',
  bin: 'SHL01',
  consumable: false,
  labour: false,
  stocktake: true,
  on_order: 0,
  consignment: false,
  total_allocated: 2,
  total_used: 50,
  total_purchased: 5,
  adjustments: 2,
  received: 1,
  service_used: 20,
  service_allocated: 0,
  repair_item_used: 10,
  repair_item_allocated: 0,
  tyre_item_used: 10,
  tyre_item_allocated: 0,
  equipment_issue_used: 10,
  lead_time: 5,
  archived: false,
  general_ledger_code: 'GL123 - Maintenance',
  notes: 'Oil filters for prime movers',
  created_at: '2024-05-16T11:08:07.449+10:00',
  updated_at: '2024-05-16T11:08:07.449+10:00',
  # site_parts is only present if multisite inventory is enabled for the business
  site_parts: [
    {
      site: 'Sydney',
      in_stock: 1,
      on_order: 10,
      stock_level: 1,
      reorder: 1,
      bin: 'SHL02',
      lead_time: 5,
      received: 1,
      adjustments: 1,
      total_purchased: 1,
      total_allocated: 1,
      total_used: 1,
      service_used: 1,
      service_allocated: 1,
      repair_item_used: 1,
      repair_item_allocated: 1,
      tyre_item_used: 1,
      tyre_item_allocated: 1,
      equipment_issue_used: 1,
      created_at: '2024-05-16T11:08:07.449+10:00',
      updated_at: '2024-05-16T11:08:07.449+10:00',
    }
  ]
}
```

## part.updated event

```rb
{
  id: 1,
  part_number: 'ABC123',
  alternate_part_number: 'DAF321',
  description: 'Oil Filter',
  supplier: [
    {
      name: 'Repco',
      code: 'REP123'
    }
  ],
  each: 10.10,
  reorder: 10,
  stock_level: 20,
  each_type: 'ea',
  bin: 'SHL01',
  consumable: false,
  labour: false,
  stocktake: true,
  on_order: 0,
  consignment: false,
  total_allocated: 2,
  total_used: 50,
  total_purchased: 5,
  adjustments: 2,
  received: 1,
  service_used: 20,
  service_allocated: 0,
  repair_item_used: 10,
  repair_item_allocated: 0,
  tyre_item_used: 10,
  tyre_item_allocated: 0,
  equipment_issue_used: 10,
  lead_time: 5,
  archived: false,
  general_ledger_code: 'GL123 - Maintenance',
  notes: 'Oil filters for prime movers',
  created_at: '2024-05-16T11:08:07.449+10:00',
  updated_at: '2024-05-20T11:08:07.449+10:00',
  # site_parts is only present if multisite inventory is enabled for the business
  site_parts: [
    {
      site: 'Sydney',
      in_stock: 1,
      on_order: 10,
      stock_level: 1,
      reorder: 1,
      bin: 'SHL02',
      lead_time: 5,
      received: 1,
      adjustments: 1,
      total_purchased: 1,
      total_allocated: 1,
      total_used: 1,
      service_used: 1,
      service_allocated: 1,
      repair_item_used: 1,
      repair_item_allocated: 1,
      tyre_item_used: 1,
      tyre_item_allocated: 1,
      equipment_issue_used: 1,
      created_at: '2024-05-16T11:08:07.449+10:00',
      updated_at: '2024-05-16T11:08:07.449+10:00',
    }
  ]
}
```

## part.destroyed event

```rb
{
  id: 1
}
```