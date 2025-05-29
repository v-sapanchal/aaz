# [Command] _network network-watcher packet-capture query-status_

Query the status of a running packet capture session.

## Versions

### [2024-05-01](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcmVzb3VyY2Vncm91cHMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5uZXR3b3JrL25ldHdvcmt3YXRjaGVycy97fS9wYWNrZXRjYXB0dXJlcy97fS9xdWVyeXN0YXR1cw==/2024-05-01.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/resourcegroups/{}/providers/microsoft.network/networkwatchers/{}/packetcaptures/{}/querystatus 2024-05-01 -->

### [2024-07-01](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcmVzb3VyY2Vncm91cHMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5uZXR3b3JrL25ldHdvcmt3YXRjaGVycy97fS9wYWNrZXRjYXB0dXJlcy97fS9xdWVyeXN0YXR1cw==/2024-07-01.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/resourcegroups/{}/providers/microsoft.network/networkwatchers/{}/packetcaptures/{}/querystatus 2024-07-01 -->

#### examples

- Query packet capture status
    ```bash
        network network-watcher packet-capture query-status --resource-group rg1 --network-watcher-name nw1 --packet-capture-name pc1
    ```
