Tasks
=====

0. Ensure your AWS environment is working.

1. Use `ipaas_lab_setup.ps1` to setup basic VPC, subnet, gateway, route, security group.

2. Create a queue  named `labq`

3. Create an Amazon Linux EC2 instance with the instance profile.

4. Use `git` on the instance to clone *this* repository.

5. Move `qprocessor.py` to the `/home/ec2-user` directory. (mv)

6. Run the `qprocessor.py` program so that it's printing "no messages".
   Install any additional package(s) you need using `yum` and/or `pip3`.

7. Send some messages to your queue from your lab desktop - these should be received.

8. Stop your `qprocessor.py`.

9. Install the service unit file in `/etc/systemd/system/qprocessor.service`.
	Modify to point to your queue.

10. Enable your service

11. Start your service.

12. Send messages to your queue. Do they appear in the file `qmessages.txt`?

