# SIPP test scenarios

Will be updated and documented.. someday

**examples:**

```bash
./sipp 192.168.0.1:5060 -sf scenario/REGISTER_client.xml -inf scenario/REGISTER_client.csv -m 5 -l 1 -t l1 -trace_msg -trace_err
```

### Test sip server with INVITE
```bash
./sipp example.com -sf scenario/INVITE-180-CANCEL/INVITE-recv180-CANCEL-or-BYE.xml -m 1 -s 1001 -ap test -key dnid 1001 -key domain example.com -key clid 2000 -key fromuser 2000
```

### Test proxy (Kamailio/OpenSIPs) AUTH route
```bash
./sipp example.com -sf scenario/INVITE-180-CANCEL/INVITE-recv180-CANCEL-or-BYE-domain-test.xml -m 1 -s 1001 -ap test -key dnid 1001 -key fromdomain fromdom.com -key todomain todomain.com -key clid 2000 -key fromuser 2000
```

