# logwatch

`logwatch` is an easy CLI for CloudWatch Log management

## Usage

### list logs

`logwatch list` returns all of your log groups. and `logwatch list [group name]` will return the log streams within that group.

### get

`logwatch get <group name>` returns log messages from a log group. You can optionally pass:

| long flag | short flag | description |
| --- | --- | --- |
| **--streams** | **-s** | Show logs from a specific stream (can be specified multiple times) |
| **--filter** | | The Filter pattern to apply to the logs stream|
| **--follow** | **-f** | Poll log stream and continuously print new log stream events |
| **--start** | | Start Time to return logs (e.g. -1h, 2019-01-01 11:16:50 GMT) |
| **--end** | | End time to return logs (e.g. 2030-02-28 11:00:00 GMT) |