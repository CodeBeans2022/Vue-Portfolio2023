<template>
<div class="container">
    <div class="row">
        <div class="col">
            <div class="row">
                <div class="col">
                    <div id="worklist" class="d-flex flex-column gap-2 worklist-scrollspy text-center" v-for="item in resumeWork" :key="item">
                        <a class="p-1 rounded" href="#worklist">{{ item.company }}</a>
                    </div>
                </div>
                <div class="col resume">
                    <div data-bs-spy="scroll" data-bs-target="#worklist" data-bs-offset="0" data-bs-smooth-scroll="true" class="scrollspy" tabindex="0" v-for="item in resumeWork" :key="item">
                        <h6 id="worklist">{{ item.company }}</h6>
                        <p>{{ item.occupation }}</p>
                        <p>{{ item.duration }}</p>
                        <p>{{ item.location }}</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="col">
            <div class="row">
                <div class="col">
                    <div id="educationlist" class="d-flex flex-column gap-2 educationlist-scrollspy text-center" v-for="item in resumeEducation" :key="item">
                        <a class="p-1 rounded" href="#educationlist">{{ item.institution }}</a>
                    </div>
                </div>
                <div class="col resume">
                    <div data-bs-spy="scroll" data-bs-target="#educationlist" data-bs-offset="0"
                        data-bs-smooth-scroll="true" class="scrollspy" tabindex="0">
                        <h6 id="educationlist"></h6>
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
                company: 'EXL',
                occupation: 'Back Office Verifications Agent',
                duration: 'December 2021-May 2022',
                location: 'Media 24, Foreshore, Cape Town'
            },
            {
                company: 'Rocomamas',
                occupation: 'Waitress',
                duration: 'February 2021-April 2021',
                location: `Jakes Gerwel Dr, Mitchell's Plain`
            },
            {
                company: 'Mugg & Bean',
                occupation: 'Cashier and Barista',
                duration: 'December 2020-January 2021',
                location: 'Century City, Cape Town'
            },
            {
                company: 'Shift Espresso Bar',
                occupation: 'Waitress',
                duration: 'December 2019-January 2020',
                location: 'Buitenkant Street CBD, Cape Town'
            },
            {
                company: 'Mugg & Bean',
                occupation: 'Cashier and Barista',
                duration: 'December 2018-February 2019',
                location: 'Century City'
            }
            
        ], 
      resumeEducation:  [
      {
                institution: 'Udemy',
                course: 'Online Courses',
                duration: 'Currently Completing',
                topics: 'Network +, A+, Security +'
            },
            {
                institution: 'LifeChoices Academy',
                course: 'Coding and Web-Development',
                duration: 'September-December 2021',
                location: '314 Imam Haron Road, Lansdowne'
            },
            {
                institution: 'Balco College',
                course: 'Grade 11-12',
                duration: 'January 2019-June 2021',
                location: `Portlands, Mitchell's Plain`
            },
            {
                institution: 'Westridge High School',
                course: 'Grade 10',
                duration: 'January-December 2018',
                location: `Westridge, Mitchell's Plain`
            },
            {
                institution: 'Crawford CoCT',
                course: 'Information Technology & Computer Sciences',
                duration: 'January-December 2017',
                location: 'Crawford, Cape Town'
            },
            {
                institution: 'Portland High School',
                course: 'Grade 8-9',
                duration: 'January 2015-December 2016',
                location: `Portland, Mitchell's Plain`
            }
        ]
    }
} 
}
</script>

<style scoped>
/* .container {
    overflow-y: scroll;
} */

a {
    text-decoration: none;
    color: black;
}

a:active{
  background-color: orchid;
}
</style>