# Troubleshooting Jina

## Module not found error

Be sure to run `pip install -r requirements.txt` before beginning, and ensure you have lots of RAM/swap and space in your `tmp` partition (see below issues). This may take a while since there are a lot of prerequisites to install.


## My Computer Hangs

Machine learning requires a lot of resources, and if your machine just hangs this is often due to running out of memory. To fix this, try [creating a swap file](https://linuxize.com/post/how-to-add-swap-space-on-ubuntu-20-04/) if you use Linux. This isn't such an issue on macOS, since it allocates swap automatically.


## Installing requirements fails

This can happen for many reasons. Let's look at the error message to debug:

`blah blah`: This means you need to [increase the size of your `/tmp` partition on Linux](https://askubuntu.com/questions/199565/not-enough-space-on-tmp)

## `ERROR: Could not install packages due to an EnvironmentError: [Errno 28] No space left on device`

This is often due to your `/tmp` partition running out of space so you'll need to [increase its size](https://askubuntu.com/questions/199565/not-enough-space-on-tmp).