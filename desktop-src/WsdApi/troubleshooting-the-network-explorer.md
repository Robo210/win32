---
Description: Lists the diagnostic procedures to use when troubleshooting the Network Explorer.
ms.assetid: 56052a82-d3a6-4749-9010-6796558dcb17
title: Troubleshooting the Network Explorer
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Troubleshooting the Network Explorer

The Network Explorer:

-   Always uses UDP WS-Discovery for device discovery
-   Always initiates a HTTP or HTTPS connection for metadata exchange
-   Sometimes uses a secure channel (HTTPS) for metadata exchange

The following diagnostic procedures should be used (in order) to help identify problems with the Network Explorer.

**To troubleshoot the Network Explorer**

1.  [Inspect adapter and firewall settings](inspecting-adapter-and-firewall-settings.md).
2.  [Use a generic host and client for UDP WS-Discovery](using-a-generic-host-and-client-for-udp-ws-discovery.md).
3.  [Use WSD Debug Client to verify multicast traffic](using-wsddebug-client-to-verify-multicast-traffic.md).
4.  [Inspect network traces for UDP WS-Discovery](inspecting-network-traces-for-udp-ws-discovery.md).
5.  [Use a generic host and client for HTTP metadata exchange](using-a-generic-host-and-client-for-http-metadata-exchange.md).
6.  [Use WinHTTP logging to verify Get traffic](using-winhttp-logging-to-verify-get-traffic.md).
7.  [Inspect network traces for HTTP metadata exchange](inspecting-network-traces-for-http-metadata-exchange.md).
8.  If a secure channel is used, [troubleshoot HTTPS secure channel communication](troubleshooting-https-secure-channel-communication.md).

The Network Explorer uses [Function Discovery](https://msdn.microsoft.com/library/windows/desktop/aa814070) to enumerate network devices. For more troubleshooting information, see [Troubleshooting Function Discovery Clients](troubleshooting-function-discovery-clients.md).

If the source of the problem cannot be identified using the above diagnostic procedures, follow the directions in [Enabling WSDAPI Tracing](enabling-wsdapi-tracing.md) and contact Microsoft support.

## Related topics

<dl> <dt>

[Getting Started with WSDAPI Troubleshooting](getting-started-with-wsdapi-troubleshooting.md)
</dt> <dt>

[Troubleshooting Function Discovery Clients](troubleshooting-function-discovery-clients.md)
</dt> </dl>

 

 


