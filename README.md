# Network-Automation

#### Project Description

1. Deploy simple web service on group of web services. Accept the client requests through a load balancer.

#### Requirements

1. Python3
2. Ansible
3. Cloud Servers
4. Ubuntu 20.04 LTS

#### Procedure

1. Deploy the required packages `nginx`, `php`, `php-fpm` onto webservers.
2. Deploy the default `nginx` template onto webservers.
3. Restart the `nginx` servers.
4. Deploy the required package `haproxy` on the group of load-balancers (here we have only one load-balancer).
5. Configure the haproxy server through editing `haproxy.cfg` configuration.
6. Restart the `haproxy` server.
7. Command to run the playbook
    -   ```
            ansible-playbook -i hosts site.yaml
        ```
8. Testing: A basic test was written at the end of the playbook which pings the load-balancer thrice and we can check whether we are getting desired output.
