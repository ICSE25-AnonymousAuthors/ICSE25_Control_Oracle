# Improved fuzzing

This is the improved fuzzing framework to create **critical scenarios** more effectively.

 - First, set up the fuzzing enviroment as guided in [Drivefuzz](https://gitlab.com/s3lab-code/public/drivefuzz/-/tree/master/).

 - Then, replace the _.py_ files under [src](https://gitlab.com/s3lab-code/public/drivefuzz/-/tree/master/src) with the files under the **src** folder here. The key design of the fuzzing framework, as well as our enhancements locate in _fuzzer.py_ and _fuzz_utils.py_.

 - Finally, the improved fuzzing framework can by activated by running the updated _fuzzer.py_. The setup process is consistant with Drivefuzz. Specifically:

   ```
   $ cd ~/drivefuzz/src
   $ ./fuzzer.py -o out-artifact -s seed-artifact -c 5 -m 5 -t behavior --timeout 60 --town 1 --strategy all
   ```


More guidance can be found in [Drivefuzz](https://gitlab.com/s3lab-code/public/drivefuzz).

