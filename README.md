# Hystrix Dashboard

This is a dashboard for monitoring applications using Hystrix (https://github.com/Netflix/Hystrix).

This project previously was a part of the [Netflix/Hystrix](https://github.com/Netflix/Hystrix) project. It is now deprecated and no longer supported. See the below security section for necessary security considerations.

View the [Dashboard Wiki](https://github.com/Netflix-Skunkworks/hystrix-dashboard/wiki) for more information including installation instructions.

<img src="https://github.com/Netflix/Hystrix/wiki/images/dashboard-home.png">


# Security

Hystrix dashboard is not intended to be deployed on untrusted networks, or without external authentication and authorization. Specifically, hystrix-dashboard does not offer any default security protection and can perform server side requests based on user provided urls.

A security advisory exist for hystrix-dashboard at [nflx-2018-001](https://github.com/Netflix/security-bulletins/blob/master/advisories/nflx-2018-001.md)


# Run via Gradle

```
$ git clone https://github.com/Netflix/Hystrix.git
$ cd Hystrix/hystrix-dashboard
$ ./gradlew appRun
> Building > :appRun > Running at http://localhost:7979/hystrix-dashboard
```

Once running, open <a href="http://localhost:7979/hystrix-dashboard">http://localhost:7979/hystrix-dashboard</a>.

# Run as standalone Java application

@kennedyoliveira has written a standalone app, documented at : https://github.com/kennedyoliveira/standalone-hystrix-dashboard

# Example

Example screenshot from iPad while monitoring Netflix API:

<center><img src="https://github.com/Netflix/Hystrix/wiki/images/hystrix-dashboard-netflix-api-example-iPad.png"></center>
