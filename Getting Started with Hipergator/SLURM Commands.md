## Some helpful [SLURM commands](https://help.rc.ufl.edu/doc/SLURM_Commands)

1. Check Job/ Queue Status
   * check jobs submitted by you: `squeue -u login`
   * check jobs submitted by everyone in group: `sbatch -A group_name1`

3. Submit a Job: `sbatch script`

4. Cancelling a Job: `scancel jobID`

5. Start Interactive Session: srun <resources> --pty bash -i
  * example: `srun --ntasks=1 --cpus-per-task=2 --mem=2gb -t 90 --pty bash -i`