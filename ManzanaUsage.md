# Manzana Usage #

```
private iPhone phone;

this.phone = new iPhone();
this.phone.Connect += new ConnectEventHandler(this.DeviceConnected);
this.phone.Disconnect += new ConnectEventHandler(this.DeviceDisconnected);
this.phone.RecoveryModeEnter += new EventHandler(this.DeviceEnterRecovery);
this.phone.RecoveryModeLeave += new EventHandler(this.DeviceLeaveRecovery);

/*
    Events
*/
private void DeviceConnected(object sender, ConnectEventArgs args)
{
    //
}
...

/*
    Getting information about the device
*/
this.phone.DeviceName - Returns the name of the device, like "Dan's iPhone".
this.phone.DeviceType - Returns the type of the device, should be either 'iPhone' or 'iPod'.
this.phone.DeviceVersion - Returns the current OS version running on the device (5.0, 5.0.1, 5.1.1).
etc...
```