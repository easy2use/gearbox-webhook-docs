# Service Webhook

## service.created event

```rb
{
  id: 1,
  fleet_number: 'ABC123',
  registration: 'NSW123',
  service_type: 'A',
  service_type_alias: '10K service',
  service_number: 12,
  fault_number: 'Fault123',
  date_open: '2024-01-01',
  odometer_scheduled: 1000000,
  hours_scheduled: 1000,
  jobcard_notes: 'Carry out A service per jobcard',
  repairer_notes: 'A service completed per jobcard',
  closed: false,
  date_closed: '2024-01-01',
  hours_closed: 1000,
  odometer_closed: 1000000,
  tolerance_kms: 11000,
  tolerance_hours: 0,
  tolerance_days: 0,
  interval_kms: 10000,
  interval_hours: 0,
  interval_days: 0,
  actual_interval_kms: 10000,
  actual_interval_hours: 0,
  actual_interval_days: 0,
  kms_ontime_status: 'on_time',
  hours_ontime_status: 'no_tolerance_set',
  days_ontime_status: 'no_tolerance_set',
  tax: 0.0,
  cost: 0.0,
  purchase_order: 'PO-123',
  invoice: 'INV123',
  invoice_date: '2024-01-01',
  location: 'Sydney',
  date_scheduled: '2024-05-16T11:08:07.449+10:00',
  date_scheduled_end: '2024-05-17T11:08:07.449+10:00',
  created_at: '2024-05-16T11:08:07.449+10:00',
  updated_at: '2024-05-16T11:08:07.449+10:00',
  site: 'Sydney',
  general_ledger_code: '1100 - Maintenance & Services',
  repairers: [
    {
      name: 'Services r Us',
      code: 'SRU'
    }
  ],
  parts: [
    {
      part_number: 'O321F123',
      part_description: 'Oil Filter',
      quantity: 1,
      each: 0,
      total: 0,
      tax: 0
    }
  ],
  labour_times: [
    {
      user: 'Internal Mechanic',
      start_time: '2024-05-16T11:08:07.449+10:00',
      end_time: '2024-05-16T11:10:07.449+10:00',
      hours: 2,
      total: 0,
      tax: 0
    }
  ]
}
```

## service.updated event

```rb
{
  id: 1,
  fleet_number: 'ABC123',
  registration: 'NSW123',
  service_type: 'A',
  service_type_alias: '10K service',
  service_number: 12,
  fault_number: 'Fault123',
  date_open: '2024-01-01',
  odometer_scheduled: 1000000,
  hours_scheduled: 1000,
  jobcard_notes: 'Carry out A service per jobcard',
  repairer_notes: 'A service completed per jobcard',
  closed: false,
  date_closed: '2024-01-01',
  hours_closed: 1000,
  odometer_closed: 1000000,
  tolerance_kms: 11000,
  tolerance_hours: 0,
  tolerance_days: 0,
  interval_kms: 10000,
  interval_hours: 0,
  interval_days: 0,
  actual_interval_kms: 10000,
  actual_interval_hours: 0,
  actual_interval_days: 0,
  kms_ontime_status: 'on_time',
  hours_ontime_status: 'no_tolerance_set',
  days_ontime_status: 'no_tolerance_set',
  tax: 0.0,
  cost: 0.0,
  purchase_order: 'PO-123',
  invoice: 'INV123',
  invoice_date: '2024-01-01',
  location: 'Sydney',
  date_scheduled: '2024-05-16T11:08:07.449+10:00',
  date_scheduled_end: '2024-05-17T11:08:07.449+10:00',
  created_at: '2024-05-16T11:08:07.449+10:00',
  updated_at: '2024-05-16T11:08:07.449+10:00',
  site: 'Sydney',
  general_ledger_code: '1100 - Maintenance & Services',
  repairers: [
    {
      name: 'Services r Us',
      code: 'SRU'
    }
  ],
  parts: [
    {
      part_number: 'O321F123',
      part_description: 'Oil Filter',
      quantity: 1,
      each: 0,
      total: 0,
      tax: 0
    }
  ],
  labour_times: [
    {
      user: 'Internal Mechanic',
      start_time: '2024-05-16T11:08:07.449+10:00',
      end_time: '2024-05-16T11:10:07.449+10:00',
      hours: 2,
      total: 0,
      tax: 0
    }
  ]
}
```

## service.destroyed event

```rb
{
  id: 1
}
```