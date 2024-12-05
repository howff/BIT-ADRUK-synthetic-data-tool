# Convert from notebook to Python
```
pip install jupyter
jupyter-nbconvert --to python BIT_+_ADR_UK_synth_data.ipynb
```
# Install requirements (use latest version, not those in requirements.txt)
```
pip install numpy pandas
```
# Modify script to accept command line parameter
```
sed -i 's/file_path = ""/import sys\nfile_path = sys.argv[1]/' BIT_+_ADR_UK_synth_data.py
```
# Run script
```
python _ADR_UK_synth_data.py test.csv
```
