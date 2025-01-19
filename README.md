<<<<<<< HEAD
# Employeemanagerfrontend

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 17.0.3.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
=======
# EmployemenetFrontend
>>>>>>> origin/main
>>>>>/home/gautamjaganatha/Downloads/Performing-OCR-main/src/main/resources/documents
>>>>>Error opening data file /usr/local/share/tessdata/eng.traineddata
Please make sure the TESSDATA_PREFIX environment variable is set to your "tessdata" directory.
Failed loading language 'eng'
Tesseract couldn't load any languages!
#
# A fatal error has been detected by the Java Runtime Environment:
#
#  SIGSEGV (0xb) at pc=0x0000f37b6fa92ccc, pid=10332, tid=0x0000f37b787ff1a0
#
# JRE version: OpenJDK Runtime Environment (8.0_432) (build 1.8.0_432-8u432-ga~us1-0ubuntu2~24.04-ga)
# Java VM: OpenJDK 64-Bit Server VM (25.432-bga mixed mode linux-aarch64 compressed oops)
# Problematic frame:
# C  [libtesseract.so.5.0.3+0x92ccc]  tesseract::Tesseract::recog_all_words(tesseract::PAGE_RES*, tesseract::ETEXT_DESC*, tesseract::TBOX const*, char const*, int)+0x3dc
#
# Failed to write core dump. Core dumps have been disabled. To enable core dumping, try "ulimit -c unlimited" before starting Java again
#
# An error report file with more information is saved as:
# /home/gautamjaganatha/Downloads/Performing-OCR-main/hs_err_pid10332.log
#
# If you would like to submit a bug report, please visit:
#   http://bugreport.java.com/bugreport/crash.jsp
# The crash happened outside the Java Virtual Machine in native code.
# See problematic frame for where to report the bug.
#




sudo apt install tesseract-ocr-eng

Set the TESSDATA_PREFIX environment variable:

echo 'export TESSDATA_PREFIX=/usr/share/tesseract-ocr/4.00/tessdata/' >> ~/.bashrc
source ~/.bashrc

Verify the language files exist:

ls /usr/share/tesseract-ocr/4.00/tessdata/eng.traineddata
If the file isn't there, you can also check:
bashCopyls /usr/share/tessdata/eng.traineddata

If you still don't see the file, you can manually download it:

sudo wget https://github.com/tesseract-ocr/tessdata/raw/main/eng.traineddata -O /usr/share/tesseract-ocr/4.00/tessdata/eng.traineddata

Process finished with exit code 134 (interrupted by signal 6:SIGABRT)
