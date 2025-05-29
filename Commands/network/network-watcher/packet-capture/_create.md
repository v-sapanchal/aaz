# [Command] _network network-watcher packet-capture create_

Create and start a packet capture on the specified VM and VMSS

## Versions

### [2024-05-01](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcmVzb3VyY2Vncm91cHMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5uZXR3b3JrL25ldHdvcmt3YXRjaGVycy97fS9wYWNrZXRjYXB0dXJlcy97fQ==/2024-05-01.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/resourcegroups/{}/providers/microsoft.network/networkwatchers/{}/packetcaptures/{} 2024-05-01 -->

### [2024-07-01](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcmVzb3VyY2Vncm91cHMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5uZXR3b3JrL25ldHdvcmt3YXRjaGVycy97fS9wYWNrZXRjYXB0dXJlcy97fQ==/2024-07-01.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/resourcegroups/{}/providers/microsoft.network/networkwatchers/{}/packetcaptures/{} 2024-07-01 -->

#### examples

- Create packet capture
    ```bash
        network network-watcher packet-capture create --resource-group rg1 --network-watcher-name nw1 --packet-capture-name pc1 --target /subscriptions/subid/resourceGroups/rg2/providers/Microsoft.Compute/virtualMachines/vm1 --bytes-to-capture-per-packet 10000 --total-bytes-per-session 100000 --time-limit-in-seconds 100 --storage-location "{storage-id:/subscriptions/subid/resourceGroups/rg2/providers/Microsoft.Storage/storageAccounts/pcstore,storage-path:'https://mytestaccountname.blob.core.windows.net/capture/pc1.cap',file-path:'D:\\capture\\pc1.cap'}" --filters "[{protocol:TCP,local-ip-address:10.0.0.4,local-port:80}]"
        network network-watcher packet-capture create --network-watcher-name "nwName" --packet-capture-name "clitestpcap1" --resource-group "NetworkWatcherRG" --storage-location '{\"localPath\":\"C:\\Captures\\testByCli.cap\"}' --target "/subscriptions/subid/resourceGroups/rgName/providers/Microsoft.Compute/virtualMachineScaleSets/testvmss" --continuous-capture false --capture-settings '{\"FileCount\":\"10\"}'
    ```
