# Fault Report Webhook

## fault_report.created event

```rb
    {
      id: 1, # unique ID of the Fault Report
      employee: 'John Smith',
      fault_date: 'Sun, 11 Sep 2022 22:17:25.329000000 UTC +00:00',
      fault_type: 'Body',
      failed_item: '',
      fail_reason: '',
      third_party_fail_reason: '',
      registration: 'ABC123',
      fleet_number: 'PM-01',
      make: "Honda",
      model: "Model A",
      archived: false,
      action: {
        type: 'Repair',
        number: 'R-123',
        notes: ''
      },
      linked_prestarts: [
        {
          prestart: "P-123"
        }
      ]
    }
```

## fault_report.updated event

```rb
    {
      id: 1, # unique ID of the Fault Report
      employee: 'John Smith',
      fault_date: 'Sun, 11 Sep 2022 22:17:25.329000000 UTC +00:00',
      fault_type: 'Body',
      failed_item: '',
      fail_reason: '',
      third_party_fail_reason: '',
      registration: 'ABC123',
      fleet_number: 'PM-01',
      make: "Honda",
      model: "Model A",
      archived: false,
      action: {
        type: 'Repair',
        number: 'R-123',
        notes: ''
      },
      linked_prestarts: [
        {
          prestart: "P-123"
        }
      ]
    }
```