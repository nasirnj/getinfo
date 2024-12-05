- name: Checking vm info
  hosts: All
  tasks:
    - name: get CPU and MEM info
      shell:
        - cat /etc/red
        - lscpu | grep "CPU(s):" | head -1
        - free -h  | awk -F ":" '{print $2}'| awk '{print $1}' | head -2 | tail -1
      
