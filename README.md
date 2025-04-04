# hsa13-hw25-s3
Create bucket where objects can’t be modified and all requests are logged.

Main bucket name: `hsa13-hw25`  
Logging bucket name: `hsa13-hw25-logs`

---
- **Object Lock** was enabled during bucket creation
- **Default retention** is set to `Compliance` mode for 1 day
- **Versioning** is enabled for the bucket
- Server access logging is **enabled** for the bucket `hsa13-hw25`
- Logs are sent to the bucket `hsa13-hw25-logs`
---

## Deletion Behavior

- When deleting an object, a **delete marker** is created
- The **actual object version remains protected** due to `Compliance` mode
- This ensures the object **cannot be modified or permanently deleted**
