Expected output:

```
PLAY [Parsing network outputs] *************************************************

TASK [Parse Aruba output] ******************************************************
ok: [localhost]

TASK [Get total bytes of a given port] *****************************************
ok: [localhost] => (item={'port': '1/1', 'total_bytes': '0', 'total_frames': '0', 'errors_rx': '0', 'drops_tx': '0', 'flow_ctrl': 'off', 'bcast_limit': '0'}) => {
    "msg": "OK to shutdown port 1/1"
}
skipping: [localhost] => (item={'port': '1/2', 'total_bytes': '12,345,678', 'total_frames': '123,456', 'errors_rx': '0', 'drops_tx': '0', 'flow_ctrl': 'off', 'bcast_limit': '0'}) 
ok: [localhost] => (item={'port': '1/3', 'total_bytes': '0', 'total_frames': '0', 'errors_rx': '0', 'drops_tx': '0', 'flow_ctrl': 'off', 'bcast_limit': '0'}) => {
    "msg": "OK to shutdown port 1/3"
}

PLAY RECAP *********************************************************************
localhost                  : ok=2    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   

```
