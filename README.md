# Magento 2 Fedex Preference

> Magento 2.3.6 Fedex Preference to remove the insurance upcharge. 

Plugin does not work because this is a protected function. 

The 2 changes are:

```
'TotalInsuredValue' => ['Amount' => '0.00', 'Currency' => $this->getCurrencyCode()],
```

```
$ratesRequest['RequestedShipment']['RequestedPackageLineItems'][0]['InsuredValue'] = [
   'Amount' => '0.00',
   'Currency' => $this->getCurrencyCode(),
];
```            
