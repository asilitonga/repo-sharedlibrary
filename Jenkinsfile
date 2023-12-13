//menggunakan shared library dari folder: vars
@Library("library-sharednya@master")_
//menggunakan shared library dari folder: src
import fungsi-echo.materi-echo.Output;

pipeline {
    agent any
    stages {
        //menggunakan folder: src (developer)
        stage ("panggil file shared-library srcnya") {
            steps {
                script {
                    Output.hello("Developer")
                }
            }
        }

        stage ("panggil file shared-library varsnya") {
            steps {
            //cara panggilnya dengan instruksi SCRIPT: namafile + nama function()
            //dibawah instruksi script kita tinggal panggil namenya BUKAN PAKAI ECHO LAGI
                script {
                    hello.world()
                }
            }
        }
    }
}