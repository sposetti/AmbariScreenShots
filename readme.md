Ambari Admin View
---

Follow the instructions here to ease frontend development for the Admin View (`ambari-admin` module)

1. Follow the [Quick Start Guide](https://cwiki.apache.org/confluence/display/AMBARI/Quick+Start+Guide) to install and start Ambari Server (cluster need not be deployed).
2. Follow the "Frontend Development" section in [Quick Start Guide](https://cwiki.apache.org/confluence/display/AMBARI/Quick+Start+Guide) to check out the Ambari source using git. This makes the entire Ambari source available via /vagrant/ambari from the Vagrant VM.
3. From the Ambari Server host:
        cd /var/lib/ambari-server/resources/views/work
> Note: If this directory does not exist, you have not started ambari-server; run "ambari-server start" to start it
4. Move the existing Admin View working directory to tmp:
    mv ADMIN_VIEW\{1.0.0\} /tmp
5. Create a symbolic link to your 
    ln -s /vagrant/ambari/ambari-admin/src/main/resources/ui/admin-web/dist ADMIN_VIEW\{1.0.0\}
6. Copy the existing view definition file in place:
    cp /tmp/ADMIN_VIEW\{1.0.0\}/view.xml ADMIN_VIEW\{1.0.0\} 
7. Restart Ambari Server for the changes to take affect:
    ambari-server restart

Now you can change the source code for Admin View and run gulp locally, and the changes are automatically reflected on the server.
