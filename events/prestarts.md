# Prestart Webhook

## prestart.created event

```rb
{
  id: 1, # unique ID of the Prestart
  prestart_number: 100,
  fleet_number: 'PM-01',
  registration: 'ABC123',
  completed_by: 'Jane Doe',
  completed_at: '2023-12-11T14:17:33.283+11:00',
  created_at: '2023-12-11T14:17:33.283+11:00',
  hours: 1000,
  mileage: 10000,
  spare1: 'Notes for spare 1',
  spare2: 'Notes for spare 2',
  spare3: 'Notes for spare 3',
  questions: [
    {
      question: 'I am fit for duty and not under the influence of drugs or alcohol',
      fail_reason: '',
      status: 'passed',
      notes: ''
    }
  ]
}
```