@Library("library-sharednya@main")_

pipeline {
    agent any
    stages {
        stage ("panggil file shared-librarynya") {
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