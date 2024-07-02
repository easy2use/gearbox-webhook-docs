# Purchase Order Webhook

## purchase_order.created event

```rb
{
  id: 1 # unique ID of the purchase order,
  supplier: 'Trucks R Us',
  vehicle_group: 'Sydney',
  purchase_order_date: 2020-01-01,
  created_by: 'John Smith',
  approved: true,
  approved_user: 'Jane Doe',
  approved_date: 2020-02-01,
  invoice: 'ABC123',
  invoice_date: 2020-03-01,
  reference_number: 'PO-1234',
  instructions: 'Please supply per instructions',
  cost: 100.00,
  tax: 9.09,
  actual_cost: 100.00,
  actual_tax: 9.09,
  tax_rate: 'Inclusive',
  closed: true,
  bulk_receive_date: 2020-02-01,
  vehicle: 'PM01',
  general_ledger_code: '123 - GL Code',
  purchase_order_number: 'PO-123',
  linked_service: '123',
  linked_repair: '123',
  linked_tyre: '123',
  linked_other: '123',
  purchase_order_items: [
    {
        id: 1,
        part_number: 'DSA123',
        part_description: 'Oil filters',
        quantity: 1,
        each_price: 10.00,
        total: 10.00,
        tax: 9.09,
        tax_percent: 10,
        tax_rate: 'Inclusive',
        tax_code: 'GST Free',
        invoice: 'ABC123',
        received_quantity: 1,
        received_date: 2020-02-01,
        site: 'Sydney',
        general_ledger_code: '123 - GL Code'
    }
  ],
  attachments: [
    {
      id: 1,
      filename: 'quote.pdf',
      content_type: 'application/pdf',
      content_length: 6398915,
      # base64_content has been truncated for brevity
      base64_content: 'iVBORw0KGgoAAAANSUhEUgAAAXUAAAKbCAYAAAAKWxqnAAAK5mlDQ1BJQ0MgUHJvZmlsZQAASImVlwdUU9kWhs+',
      created_at: 2020-01-01,
      updated_at: 2020-01-01
    }
  ]
}
```

## purchase_order.updated event

```rb
{
  id: 1 # unique ID of the purchase order,
  supplier: 'Trucks R Us',
  vehicle_group: 'Sydney',
  purchase_order_date: 2020-01-01,
  created_by: 'John Smith',
  approved: true,
  approved_user: 'Jane Doe',
  approved_date: 2020-02-01,
  invoice: 'ABC123',
  invoice_date: 2020-03-01,
  reference_number: 'PO-1234',
  instructions: 'Please supply per instructions',
  cost: 100.00,
  tax: 9.09,
  actual_cost: 100.00,
  actual_tax: 9.09,
  tax_rate: 'Inclusive',
  closed: true,
  bulk_receive_date: 2020-02-01,
  vehicle: 'PM01',
  general_ledger_code: '123 - GL Code',
  purchase_order_number: 'PO-123',
  linked_service: '123',
  linked_repair: '123',
  linked_tyre: '123',
  linked_other: '123',
  purchase_order_items: [
    {
        id: 1,
        part_number: 'DSA123',
        part_description: 'Oil filters',
        quantity: 1,
        each_price: 10.00,
        total: 10.00,
        tax: 9.09,
        tax_percent: 10,
        tax_rate: 'Inclusive',
        tax_code: 'GST Free',
        invoice: 'ABC123',
        received_quantity: 1,
        received_date: 2020-02-01,
        site: 'Sydney',
        general_ledger_code: '123 - GL Code'
    }
  ],
  attachments: [
    {
      id: 1,
      filename: 'quote.pdf',
      content_type: 'application/pdf',
      content_length: 6398915,
      # base64_content has been truncated for brevity
      base64_content: 'iVBORw0KGgoAAAANSUhEUgAAAXUAAAKbCAYAAAAKWxqnAAAK5mlDQ1BJQ0MgUHJvZmlsZQAASImVlwdUU9kWhs+',
      created_at: 2020-01-01,
      updated_at: 2020-01-01
    }
  ]
}
```

## purchase_order.destroyed event

```rb
{
  id: 1 # unique ID of the purchase order
}
```