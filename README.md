Hyper-V provisioning
========================

**Objetivo**
-------------

Provisionar máquinas virtuais no Hyper-V utilizando templates de sistemas operacionais Linux ou Windows.

**Funções**
-------------

- [X] Cria a estrutura de diretórios necessária: Organiza as pastas para armazenar o VHDX e a VM.

- [x] Valida a existência do VHDX: Verifica se o arquivo de disco virtual (VHDX) já está presente no diretório.

- [x] Cria um novo VHDX a partir do template: Duplica o VHDX template para gerar um novo disco virtual para a máquina.

- [x] Valida a existência da VM: Confirma se a máquina virtual com o nome especificado já foi criada.

- [x] Provisiona a VM utilizando o VHDX template: Cria uma nova máquina virtual a partir do template VHDX, associando o disco ao controlador adequado.

- [x] Configura a VM provisionada: Realiza configurações adicionais na VM, como alocação de recursos, adaptação de rede e personalizações necessárias para que a VM esteja pronta para uso.

**Referências**
-------------

- https://docs.ansible.com
- https://write-verbose.com/2023/08/13/HyperVDiff/
- https://github.com/tsailiming/ansible-hyperv/tree/master
- https://medium.com/tech-jobs-academy/- how-to-use-differencing-disks-to-deploy-multiple-vms-quickly-in-hyper-v-1634f94c5541
- https://learn.microsoft.com/en-us/powershell/module/hyper-v/new-vhd?view=windowsserver2025-ps
- https://learn.microsoft.com/en-us/powershell/module/hyper-v/new-vm?view=windowsserver2025-ps