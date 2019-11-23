Diese Hoodfile kann nur verwendet werden, wenn der Public Key des Routers in list.key eingetragen ist. Für jeden Key ist eine neue Zeile zu verwenden.

Der Publickey kann folgendermaßen aus dem Router ausgelesen werden:

```console
echo "secret \"$(uci get fastd.fff.secret)\";" > /tmp/sec && fastd --show-key -c /tmp/sec
```

Die SSID darf in der Hoodfile verändert werden, alle anderen Werte dürfen nicht verändert werden! Für Meshrouter muss hier kein Key hinterlegt werden, sie benötigen aber ebenfalls die gleiche Hoodfile manuell angelegt.

Die Hoodfile nach /etc/hoodfile auf den Router kopieren.
