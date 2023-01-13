<template>
<div class="container mt-5 ">
<div class="row">
    <div class="col">
        <h1 class="mb-5">Work Experience</h1>
    </div>
    <div class="col">
        <h1 class="mb-5">Education Experience</h1>
    </div>
</div>

    <div class="row">
        <div class="col">
            <div class="row">
                <div class="col">
                    <div id="worklist" class="d-flex flex-column gap-2 worklist-scrollspy text-center" v-for="item in resumeWork" :key="item">
                        <a class="p-1 rounded mb-3" :href="'#' + item.id">{{ item.company }}</a>
                    </div>
                </div>
                <div class="col resume">
                    <div  data-bs-spy="scroll" data-bs-target="#worklist" data-bs-offset="0" data-bs-smooth-scroll="true" class="scrollspy" tabindex="0" v-for="item in resumeWork" :key="item" :id="item.id">
                        <table class="table">
                            <tr>
                                <th scope="row">Company</th>
                                <td>{{ item.company }}</td>
                            </tr>
                            <tr>
                                <th scope="row">Occupation</th>
                                <td>{{ item.occupation }}</td>
                            </tr>
                            <tr>
                                <th scope="row">Duration</th>
                                <td>{{ item.duration }}</td>
                            </tr>
                            <tr>
                                <th scope="row">Location</th>
                                <td>{{ item.location }}</td>
                            </tr>
                        </table>
                    </div>
                </div>
            </div>
        </div>

        <div class="col">
            <div class="row">
                <div class="col">
                    <div id="educationlist" class="d-flex flex-column gap-2 worklist-scrollspy text-center" v-for="item in resumeEducation" :key="item">
                        <a class="p-1 rounded mb-3" :href="'#' + item.id">{{ item.institution }}</a>
                    </div>
                </div>
                <div class="col resume">
                    <div data-bs-spy="scroll" data-bs-target="#educationlist" data-bs-offset="0" data-bs-smooth-scroll="true" class="scrollspy" :tabindex="item.id" v-for="item in resumeEducation" :key="item" :id="item.id">
                        <table class="table">
                            <tr>
                                <th scope="row">Institution</th>
                                <td>{{ item.institution }}</td>
                            </tr>
                            <tr>
                                <th scope="row">Occupation</th>
                                <td>{{ item.course }}</td>
                            </tr>
                            <tr>
                                <th scope="row">Duration</th>
                                <td>{{ item.duration }}</td>
                            </tr>
                            <tr>
                                <th scope="row">Location</th>
                                <td>{{ item.location }}</td>
                            </tr>
                        </table>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

</template>

<script>
export default {
    name: 'Resume',
    data() {
    return{
        resumeWork: [
            {
                id: 1,
                company: 'EXL',
                occupation: 'Back Office Verifications Agent',
                duration: 'December 2021-May 2022',
                location: 'Media 24, Foreshore, Cape Town'
            },
            {
                id: 2,
                company: 'Rocomamas',
                occupation: 'Waitress',
                duration: 'February 2021-April 2021',
                location: `Jakes Gerwel Dr, Mitchell's Plain`
            },
            {
                id: 3,
                company: 'Mugg & Bean',
                occupation: 'Cashier and Barista',
                duration: 'December 2020-January 2021',
                location: 'Century City, Cape Town'
            },
            {
                id: 4,
                company: 'Shift Espresso Bar',
                occupation: 'Waitress',
                duration: 'December 2019-January 2020',
                location: 'Buitenkant Street CBD, Cape Town'
            },
            {
                id: 5,
                company: 'Mugg & Bean',
                occupation: 'Cashier and Barista',
                duration: 'December 2018-February 2019',
                location: 'Century City'
            }
            
        ], 
      resumeEducation:  [
            {
                id: 6,
                institution: 'Udemy',
                course: 'Network +, A+, Security +',
                duration: 'Currently Completing',
                location: 'Online Platform'
            },
            {
                id: 7,
                institution: 'LifeChoices Academy',
                course: 'Coding and Web-Development',
                duration: 'September-December 2021',
                location: '314 Imam Haron Road, Lansdowne'
            },
            {
                id: 8,
                institution: 'Balco College',
                course: 'Grade 11-12',
                duration: 'January 2019-June 2021',
                location: `Portlands, Mitchell's Plain`
            },
            {
                id: 9,
                institution: 'Westridge High School',
                course: 'Grade 10',
                duration: 'January-December 2018',
                location: `Westridge, Mitchell's Plain`
            },
            {
                id: 10,
                institution: 'Crawford CoCT',
                course: 'Information Technology & Computer Sciences',
                duration: 'January-December 2017',
                location: 'Crawford, Cape Town'
            },
            {
                id: 11,
                institution: 'Portland High School',
                course: 'Grade 8-9',
                duration: 'January 2015-December 2016',
                location: `Portland, Mitchell's Plain`
            }
        ]
    }
} ,
methods: {
    function(){
        let links = document.querySelectorAll('#worklist')
    }
}
}
</script>

<style scoped>
.resume {
    overflow-y: scroll;
    height: 400px;
}

a {
    text-decoration:overline;
    color: black;
}

a:active{
  background-color: orchid;
}

.scrollspy{
    border: 2px solid black;
    margin-bottom: 20px;
    border-radius: 15px;
    padding: 10px;
}

td, th{
    border: 1px solid black;
    padding: 2px;
}




</style>