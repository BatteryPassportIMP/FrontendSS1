<template>
    <div>
        <v-divider class="app-footer-div" color="#AEE5C5" thickness="3"></v-divider>
        <v-footer class="text-center">
            <p class="app-footer-text">
                All personally identifiable information in this application will 
                be handled in accordance with the <a href="https://gdpr-info.eu/">
                GDPR</a> guidelines.
                <br>
                This project was developed in collaboration with <a href="https://www.htw-berlin.de/">University of Applied Sciences Berlin</a>
              — represented by the President Prof. Dr.  Annabella Rauscher Disc —
            </p>
        </v-footer>
    </div>
    
</template>

<style scoped>
.app-footer-div {
    margin-left: 2%;
    margin-right: 2%;
    margin-bottom: 0.5%;
}

.app-footer-text {
    line-height: 1.2;
    font-size: small;
    margin-bottom: 0.5%;
    text-align: center;
    margin-left: auto;
    margin-right: auto;
}
</style>