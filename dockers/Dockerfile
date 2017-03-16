# docker build -t gromacs .

FROM lipcomputing/nvidia-ubuntu16.04:nvdrv_375.26
MAINTAINER Mario David <mariojmdavid@gmail.com>
LABEL description="Run Gromacs application"

RUN ansible-galaxy install git+https://github.com/LIP-Computing/ansible-role-gromacs.git && \
    ansible-playbook /etc/ansible/roles/ansible-role-gromacs/tests/gromacs.yml

ENV PATH /usr/local/cuda-8.0/bin:$PATH
ENV LD_LIBRARY_PATH /usr/local/cuda-8.0/lib64:$LD_LIBRARY_PATH
CMD ["/bin/bash","-c",". /usr/local/gromacs/bin/GMXRC.bash"]
