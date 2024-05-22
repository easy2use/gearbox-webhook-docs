# Repair Webhook

## repair.created event

```rb
{
  id: 2340261, 
  repair_number: 1739
  date_reported: '2024-05-16'
  fault_number: 'Fault123'
  fleet_number: 'ABC123'
  registration: 'NSW123'
  reported_to: 'John Smith'
  reported_by: 'Jane Doe'
  location: 'Sydney'
  job_number: 'JOB123'
  defect: 'DEFECT123'
  defect_cleared_by_date: '2024-05-16'
  defect_cleared_by: 'Defects r Us'
  odometer_open: 1000000
  hours_open: 1000
  created_at: '2024-05-16T11:08:07.449+10:00'
  updated_at: '2024-05-16T11:21:02.042+10:00'
  purchase_order: 'PO123'
  site: 'Sydney'
  repair_items: [
    {
      problem: 'Cracked windshield'
      notes: 'Stone chip'
      repairer_notes: 'Replaced windshield'
      assigned_user: 'Mechanic'
      invoice: 'INV123'
      invoice_date: '2024-05-16'
      cost: 10.0
      tax: 0.91
      general_ledger_code: '1100 - Repairs' 
      date_closed: '2024-05-16'
      odometer_closed: 1000000
      hours_closed: 1000
      status: open
      priority: normal
      repairers: [
        {
          code: 'ABC123',
          name: 'Windshields r Us'
        }
      ]
      repair_types: [
        {
          type: 'Defect'
        }
      ]
      parts: [
        {
          part_number: 'ABC123'
          part_description: 'Windshield'
          quantity: 1
          each: 1
          total: 0.0
          tax: 0.0
        }
      ]
      labour_times: [
        {
          user: 'Mechanic'
          start_time: '2024-05-16T10:51:01.987+10:00'
          end_time: '2024-05-16T11:21:01.987+10:00'
          hours: 0.5
          total: 10.0
          tax: 0.91
        }
      ]
    }
  ]
}
```

## repair.updated event

```rb
{
  id: 2340261, 
  repair_number: 1739
  date_reported: '2024-05-16'
  fault_number: 'Fault123'
  fleet_number: 'ABC123'
  registration: 'NSW123'
  reported_to: 'John Smith'
  reported_by: 'Jane Doe'
  location: 'Sydney'
  job_number: 'JOB123'
  defect: 'DEFECT123'
  defect_cleared_by_date: '2024-05-16'
  defect_cleared_by: 'Defects r Us'
  odometer_open: 1000000
  hours_open: 1000
  created_at: '2024-05-16T11:08:07.449+10:00'
  updated_at: '2024-05-16T11:21:02.042+10:00'
  purchase_order: 'PO123'
  site: 'Sydney'
  repair_items: [
    {
      problem: 'Cracked windshield'
      notes: 'Stone chip'
      repairer_notes: 'Replaced windshield'
      assigned_user: 'Mechanic'
      invoice: 'INV123'
      invoice_date: '2024-05-16'
      cost: 10.0
      tax: 0.91
      general_ledger_code: '1100 - Repairs' 
      date_closed: '2024-05-16'
      odometer_closed: 1000000
      hours_closed: 1000
      status: open
      priority: normal
      repairers: [
        {
          code: 'ABC123',
          name: 'Windshields r Us'
        }
      ]
      repair_types: [
        {
          type: 'Defect'
        }
      ]
      parts: [
        {
          part_number: 'ABC123'
          part_description: 'Windshield'
          quantity: 1
          each: 1
          total: 0.0
          tax: 0.0
        }
      ]
      labour_times: [
        {
          user: 'Mechanic'
          start_time: '2024-05-16T10:51:01.987+10:00'
          end_time: '2024-05-16T11:21:01.987+10:00'
          hours: 0.5
          total: 10.0
          tax: 0.91
        }
      ]
    }
  ]
}
```

## repair.destroyed event

```rb
{
  id: 1
}
```