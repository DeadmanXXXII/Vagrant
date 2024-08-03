# Vagrant
Vagrant CLI commands
Here is a comprehensive list of Vagrant CLI commands, including basic commands, advanced operations, and useful configurations.

### **Vagrant CLI Commands**

#### **1. Basic Commands**

- **Initialize a new Vagrant project:**
  ```bash
  vagrant init [BOX_NAME]
  ```

- **Start and provision the Vagrant environment:**
  ```bash
  vagrant up
  ```

- **Halt the Vagrant environment:**
  ```bash
  vagrant halt
  ```

- **Suspend the Vagrant environment (saves the state):**
  ```bash
  vagrant suspend
  ```

- **Resume a suspended Vagrant environment:**
  ```bash
  vagrant resume
  ```

- **Destroy the Vagrant environment (removes all traces):**
  ```bash
  vagrant destroy
  ```

- **Reload the Vagrant environment (reboots and applies configuration changes):**
  ```bash
  vagrant reload
  ```

- **SSH into the Vagrant box:**
  ```bash
  vagrant ssh
  ```

- **Check the status of the Vagrant environment:**
  ```bash
  vagrant status
  ```

- **Provision the Vagrant environment without starting it:**
  ```bash
  vagrant provision
  ```

#### **2. Configuration and Management**

- **Validate the Vagrantfile:**
  ```bash
  vagrant validate
  ```

- **List available boxes:**
  ```bash
  vagrant box list
  ```

- **Add a new box:**
  ```bash
  vagrant box add BOX_NAME [BOX_URL]
  ```

- **Remove a box:**
  ```bash
  vagrant box remove BOX_NAME
  ```

- **Update the Vagrant box:**
  ```bash
  vagrant box update
  ```

- **Show information about the current box:**
  ```bash
  vagrant box info BOX_NAME
  ```

- **Show detailed information about the current environment:**
  ```bash
  vagrant global-status
  ```

- **Package the Vagrant box:**
  ```bash
  vagrant package [OPTIONS]
  ```

- **Upload a package to Vagrant Cloud:**
  ```bash
  vagrant cloud publish [OPTIONS]
  ```

- **Download a Vagrant box from Vagrant Cloud:**
  ```bash
  vagrant cloud box add [OPTIONS]
  ```

#### **3. Plugin Management**

- **List installed plugins:**
  ```bash
  vagrant plugin list
  ```

- **Install a plugin:**
  ```bash
  vagrant plugin install PLUGIN_NAME
  ```

- **Update a plugin:**
  ```bash
  vagrant plugin update PLUGIN_NAME
  ```

- **Uninstall a plugin:**
  ```bash
  vagrant plugin uninstall PLUGIN_NAME
  ```

- **List available plugins:**
  ```bash
  vagrant plugin search PLUGIN_NAME
  ```

- **Update all plugins:**
  ```bash
  vagrant plugin update
  ```

#### **4. Network Commands**

- **Forward a port for the Vagrant box:**
  ```bash
  vagrant port
  ```

- **Display the Vagrant box's SSH configuration:**
  ```bash
  vagrant ssh-config
  ```

#### **5. Provisioning and Automation**

- **Run a specific provisioning script:**
  ```bash
  vagrant provision --provision-with SCRIPT_NAME
  ```

- **Disable provisioning during `vagrant up`:**
  ```bash
  vagrant up --no-provision
  ```

- **Force provisioning on `vagrant up`:**
  ```bash
  vagrant up --provision
  ```

#### **6. Advanced Usage**

- **Snapshot a Vagrant environment (create a checkpoint):**
  ```bash
  vagrant snapshot save SNAPSHOT_NAME
  ```

- **List snapshots:**
  ```bash
  vagrant snapshot list
  ```

- **Restore a snapshot:**
  ```bash
  vagrant snapshot restore SNAPSHOT_NAME
  ```

- **Delete a snapshot:**
  ```bash
  vagrant snapshot delete SNAPSHOT_NAME
  ```

- **Push a Vagrant box to a private repository:**
  ```bash
  vagrant box add BOX_NAME --provider=PROVIDER --box-version=VERSION
  ```

### **Summary**

This list of Vagrant CLI commands covers essential tasks for managing Vagrant environments, including initialization, configuration, provisioning, and advanced operations. Use these commands to efficiently create, configure, and manage development environments with Vagrant.
