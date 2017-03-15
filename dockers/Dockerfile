# docker build -t gromacs .

FROM lipcomputing/nvidia-ubuntu16.04:nvdrv_375.26
MAINTAINER Mario David <mariojmdavid@gmail.com>
LABEL description="Run Gromacs application"

RUN ansible-galaxy install git+https://github.com/LIP-Computing/ansible-role-gromacs.git && \
    ansible-playbook /etc/ansible/roles/ansible-role-gromacs/tests/gromacs.yml
