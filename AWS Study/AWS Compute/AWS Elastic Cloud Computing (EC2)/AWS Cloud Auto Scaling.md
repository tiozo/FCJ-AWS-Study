### [[AWS EC2 Auto Scaling]]
EC2 Auto Scaling can be added as a buffer on top of your businesses.
It can add new instances to the application when necessary and terminate when no longer needed.
(Simpler term, baseline --more demands--> baseline++ --less demands--> baseline.
We should not add a tier below baseline to for cost saving as it makes your server vulnerable to any sudden traffic before dynamic scaling be effective)

You can set a group of instances.
- minimum capacity of instances that will always be running. The rest will operate when necessary.
- you can 
