Once you have copied the r scripts here is how you run it
for i in {1..13}; do
>     echo "Launching cohort index $i..."
>     Rscript run_munge_tidy_no_installs.R "$i" > logs/run_$i.out 2>&1 &
> done


You can also just run

sbatch submit_munge_tidy_array.slurm
