```
[*] Service scan wkhtmltoimage (tcp/80/http/wkhtmltoimage) ran a command which returned a non-zero exit code (1).
[-] Command: wkhtmltoimage --format png http://192.168.224.246:80/ /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_screenshot.png
[-] Error Output:
QStandardPaths: XDG_RUNTIME_DIR not set, defaulting to '/tmp/runtime-root'
Loading page (1/2)
[>                                                           ] 0%
[==================>                                         ] 30%
[=================================>                          ] 55%
Error: Failed to load http://192.168.224.246/fonts/glyphicons-halflings-regular.woff2, with network status code 203 and http status code 404 - Error transferring http://192.168.224.246/fonts/glyphicons-halflings-regular.woff2 - server replied: Not Found
[============================================================] 100%
Rendering (2/2)
[>                                                           ] 0%
[===============>                                            ] 25%
[============================================================] 100%
Done
Exit with code 1 due to network error: ContentNotFoundError


[*] Service scan wkhtmltoimage (tcp/443/http/wkhtmltoimage) ran a command which returned a non-zero exit code (1).
[-] Command: wkhtmltoimage --format png https://192.168.224.246:443/ /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_screenshot.png
[-] Error Output:
QStandardPaths: XDG_RUNTIME_DIR not set, defaulting to '/tmp/runtime-root'
Loading page (1/2)
[>                                                           ] 0%
Warning: SSL error ignored
[==================>                                         ] 30%
[===========================>                                ] 45%
Error: Failed to load https://192.168.224.246/fonts/glyphicons-halflings-regular.woff2, with network status code 203 and http status code 404 - Error transferring https://192.168.224.246/fonts/glyphicons-halflings-regular.woff2 - server replied: Not Found
[====================================================>       ] 88%
[============================================================] 100%
Rendering (2/2)
[>                                                           ] 0%
[===============>                                            ] 25%
[============================================================] 100%
Done
Exit with code 1 due to network error: ContentNotFoundError


[*] Service scan wkhtmltoimage (tcp/443/https/wkhtmltoimage) ran a command which returned a non-zero exit code (1).
[-] Command: wkhtmltoimage --format png https://192.168.224.246:443/ /home/kali/Documents/Relia/results/192.168.224.246/scans/tcp443/tcp_443_https_screenshot.png
[-] Error Output:
QStandardPaths: XDG_RUNTIME_DIR not set, defaulting to '/tmp/runtime-root'
Loading page (1/2)
[>                                                           ] 0%
Warning: SSL error ignored
[==================>                                         ] 30%
Warning: SSL error ignored
Warning: SSL error ignored
[===========================>                                ] 45%
Error: Failed to load https://192.168.224.246/fonts/glyphicons-halflings-regular.woff2, with network status code 203 and http status code 404 - Error transferring https://192.168.224.246/fonts/glyphicons-halflings-regular.woff2 - server replied: Not Found
[==================================>                         ] 57%
[============================================================] 100%
Rendering (2/2)
[>                                                           ] 0%
[===============>                                            ] 25%
[============================================================] 100%
Done
Exit with code 1 due to network error: ContentNotFoundError



```