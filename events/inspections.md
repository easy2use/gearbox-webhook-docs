# Inspection Webhook

## inspection.created event

```rb
{
  id: 146352, 
  fleet_number: 'PM03', 
  registration: 'NSW123', 
  inspection_type: 'Random Inspection', 
  inspection_number: 71, 
  odometer_open: 999999,
  hours_open: 950, 
  date_open: '2024-05-22',
  cost: 0.0, 
  tax: 0.0, 
  notes: 'Notes', 
  repairer_notes: 'Notes from repairer', 
  date_closed: '2024-05-25', 
  closed: false, 
  hours_closed: 1000, 
  odometer_closed: 1000000, 
  invoice: 'INV123', 
  invoice_date: '2024-05-22', 
  location: 'Sydney', 
  date_scheduled: '2024-05-22T10:20:02.649+10:00', 
  date_scheduled_end: '2024-05-23T10:20:02.649+10:00', 
  certificate_number: 'Cert#123', 
  external_document_reference: 'ExtDoc123', 
  external_transaction_reference: 'Ext123', 
  created_at: '2024-05-22T10:20:02.649+10:00', 
  updated_at: '2024-05-22T10:24:43.686+10:00', 
  site: 'Sydney', 
  general_ledger_code: '1100 - Inspections and Maintenance', 
  repairer: [
    { 
      code: 'IRU',
      name: 'Inspections R Us',
    }
  ], 
  labour_times: [
    {
      user: 'Jordan Watson', 
      start_time: '2024-05-22T08:23:44.330+10:00',
      end_time: '2024-05-22T10:23:44.330+10:00', 
      hours: 2.0, 
      total: 0.0, 
      tax: 0.0
    }
  ]
}
```

## inspection.updated event

```rb
{
  id: 146352, 
  fleet_number: 'PM03', 
  registration: 'NSW123', 
  inspection_type: 'Random Inspection', 
  inspection_number: 71, 
  odometer_open: 999999,
  hours_open: 950, 
  date_open: '2024-05-22',
  cost: 0.0, 
  tax: 0.0, 
  notes: 'Notes', 
  repairer_notes: 'Notes from repairer', 
  date_closed: '2024-05-25', 
  closed: false, 
  hours_closed: 1000, 
  odometer_closed: 1000000, 
  invoice: 'INV123', 
  invoice_date: '2024-05-22', 
  location: 'Sydney', 
  date_scheduled: '2024-05-22T10:20:02.649+10:00', 
  date_scheduled_end: '2024-05-23T10:20:02.649+10:00', 
  certificate_number: 'Cert#123', 
  external_document_reference: 'ExtDoc123', 
  external_transaction_reference: 'Ext123', 
  created_at: '2024-05-22T10:20:02.649+10:00', 
  updated_at: '2024-05-22T10:24:43.686+10:00', 
  site: 'Sydney', 
  general_ledger_code: '1100 - Inspections and Maintenance', 
  repairer: [
    { 
      code: 'IRU',
      name: 'Inspections R Us',
    }
  ], 
  labour_times: [
    {
      user: 'Jordan Watson', 
      start_time: '2024-05-22T08:23:44.330+10:00',
      end_time: '2024-05-22T10:23:44.330+10:00', 
      hours: 2.0, 
      total: 0.0, 
      tax: 0.0
    }
  ]
}
```

## inspection.destroyed event

```rb
{
  id: 1 # unique ID of the inspection
}
```