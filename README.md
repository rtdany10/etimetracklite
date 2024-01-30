# eTimeTrackLite - Python
Pull checkin logs from eTimeTrackLite (eSSL) using python

# Sample Code:
```
machine = eTimeTrackLite(domain="my-ip-address")
machine.set_request_body({
	"from_time": "from-time",
	"to_time": "to-time",
	"serial_no": "device-serial-no",
	"username": "web-user",
	"password": "web-user-password",
})
machine.fetch_logs()
print(machine.logs[0]) -> ['1002', '2023-12-05 07:30:30', '']
```

Use `machine.logs` to get the logs.
