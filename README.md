# Port-Filter-Driver.
To filter out the IO which goes directly into the device from disk can be monitored/modified using a port filter driver. The need of port filter is because, Storport and miniport is a call/return interface, not IRP based. storport+miniport combined is a WDM driver. It's not possible to add a filter between them because they are one entity in the device stack .
