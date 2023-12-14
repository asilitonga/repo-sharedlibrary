//menggunakan shared library dari folder: vars
@Library("library-sharednya@master")_
//menggunakan shared library dari folder: src
import classpertama.classnya.Output;

pipeline {
    agent any
    stages {

        stage ("menggunakan parameter"){
            steps {
                script {
                    echo("clean compile")
                }
            }
        }

        stage ("menggunakan function") {
            steps {
                script {
                    echo(fungsifunction.name())
                    echo(fungsifunction.role())
                    echo(fungsifunction())
                }
            }
        }


        //menggunakan folder: src (developer)
        stage ("panggil file shared-library srcnya") {
            steps {
                script {
                    Output.hello(this, "Developer")
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