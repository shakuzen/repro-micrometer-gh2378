# Micrometer issue 2378 reproducer

This project reproduces the issue mentioned in Micrometer GitHub issue 2378.

Steps to reproduce:
1) Run main class to start application
2) Wait for about 5 minutes

After some time from startup, you will notice in the DEBUG logs for reactor-netty that an infinite immediate connection retry loop is happening.