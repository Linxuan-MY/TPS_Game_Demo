# TPS Game Demo

This project now includes a Relay-backed network layer built with **Netcode for GameObjects (NGO)**.
Attach `RelayNetworkManager` to a scene object that also has a `UnityTransport` component, then call
`StartRelayHostAsync` to create a host and receive a join code, or `StartRelayClientAsync` with that
code to connect as a client. Both paths bootstrap Unity Services, authenticate anonymously, and
configure NGO to use Relay DTLS endpoints before starting the host/client peers.
