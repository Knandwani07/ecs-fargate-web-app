
6. Leave remaining settings unchanged.
7. Click Create Service.
8. Wait until the service shows a running task.

---

## 🔐 IV. Configure Security Group for Application Access

1. Open the EC2 Dashboard.
2. Navigate to Security Groups.
3. Locate the default security group associated with the ECS service.
4. Edit inbound rules.
5. Add a rule:
   - Type: HTTP
   - Source: Anywhere (IPv4)
6. Save the rules.

---

## 🌐 V. Access the Running Application

1. Return to the ECS console.
2. Open the running task under the service.
3. Scroll to the Configuration section.
4. Locate the Public IP address assigned to the task.
5. Copy the public IP.
6. Open a browser and navigate to:

http://(public-ip)

7. Confirm that the Apache HTTP Server page displaying “It works!” is visible.

---

## 🧹 VI. Clean Up Resources

1. Remove the inbound HTTP rule from the security group.
2. Delete the ECS service.
3. Deregister the task definition.
4. Delete the ECS cluster if no longer required.

---

## ✅ Conclusion

This execution guide demonstrates how to deploy a containerized web application using Amazon ECS with AWS Fargate. By following these steps, users gain practical experience with managed container orchestration, task and service configuration, networking, and secure application access without managing EC2 instances. This workflow forms a solid foundation for learning container-based application deployment on AWS.
