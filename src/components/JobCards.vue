<template>
    <div class="container-fluid">
        <div class="card mb-3 border jobPosting" v-for="(empleo, indice) in empleos" :key="indice">
            <div class="card-body p-2 p-md-3" >
                <div class="row align-items-center">
                    <div class="justify-content-center align-items-center col-md-1 col-3">
                        <img class="rounded my-logo" src="../assets/img/peaku-logo.png" alt="Logo de la empresa">
                    </div>
                    <div class="col-md-11 col-9">
                        <div class="row align-items-center">
                            <a class="text-dark stretched-link d-inline d-md-inline-flex jobLink" href="#">
                                <h5 class="card-title font-weight-bold pl-md-2 pr-md-2 mb-0 pb-0">{{ empleo.name }}</h5>
                                <section class="pl-md-2 d-inline d-md-inline-flex align-items-center text-truncate">
                                    <div class="habilidad text-truncate border border-dark text-dark text-capitalize" v-for="(hab, index) in empleo.qualifications" :key="index">
                                        {{ hab }}
                                    </div>
                                </section>
                            </a>
                        </div>
                        <div class="row pl-md-2 mt-1 flex-column flex-md-row">
                            <div class="text-truncate text-capitalize col">
                                <i class="bi bi-buildings mr-1"></i>
                                <span>{{ empleo.company }}</span>
                            </div>
                            <div class="text-truncate col">
                                <i class="bi bi-geo-alt mr-1"></i>
                                <span>{{ empleo.location }}</span>
                            </div>
                            <div class="text-truncate col">
                                <i class="bi bi-cash mr-1"></i>
                                <span>{{ empleo.salary }}</span>
                            </div>
                            <div class="d-none d-md-inline-block col">
                                <i class="bi bi-people mr-1"></i>
                                {{ empleo.vacancies }} Vacante(s)
                            </div>
                            <div class="text-truncate col">
                                <i class="bi bi-calendar3 mr-1"></i>
                                <span>{{ empleo.posting_date }}</span>
                            </div>
                            <!-- <div class="text-truncate col">
                                <i class="bi bi-cash"></i>
                                <span>{{ empleo.salary }}</span>
                            </div> -->
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name: 'JobCards',
    data() {
        return {
            empleos: [
                {
                    name: "Desarrollador Java",
                    company: "Assemblers S.A.",
                    location: "Remoto",
                    vacancies: 2,
                    qualifications: {
                        a: "Java",
                        b: "Spring MVC",
                        c: "PostgreSQL"
                    },
                    salary: "$ 3.5M - 5M COP",
                    posting_date: "11/05/2023"
                },
                {
                    name: "Desarrollador PHP",
                    company: "Developers United",
                    location: "Bogotá",
                    vacancies: 1,
                    qualifications: {
                        a: "PHP",
                        b: "Laravel",
                    },
                    salary: "$ 4M COP",
                    posting_date: "02/05/2023"
                },
                {
                    name: "Desarrollador Senior",
                    company: "Developers United",
                    location: "Medellín",
                    vacancies: 1,
                    qualifications: {
                        a: "JavaScript",
                        b: "React",
                        c: "MySQL/MariaDB"
                    },
                    salary: "$ 4M COP",
                    posting_date: "22/04/2023"
                },
                {
                    name: "Diseñador Gráfico",
                    company: "Neuro",
                    location: "Remoto",
                    vacancies: 2,
                    qualifications: {
                        a: "Diseño vectorial",
                        b: "Illustrator",
                    },
                    salary: "$ 2M COP",
                    posting_date: "22/04/2023"
                },
                {
                    name: "Enfermera Profesional",
                    company: "TuMedical",
                    location: "Barranquilla",
                    vacancies: 1,
                    qualifications: {
                        a: "Seguridad laboral",
                        b: "Lenguaje de señas",
                        c: "Min. 1 año de experiencia"
                    },
                    salary: "$ 3M - 4M COP",
                    posting_date: "10/05/2023"
                },
                {
                    name: "Asesor comercial",
                    company: "Activos S.A.",
                    location: "Cali",
                    vacancies: 10,
                    qualifications: {
                        a: "Inglés",
                        b: "Atención al usuario",
                        c: "Comunicación asertiva",
                        d: "Herramientas ofimáticas"
                    },
                    salary: "$ 2.2M COP + prestaciones y comisiones",
                    posting_date: "11/05/2023"
                },
                {
                    name: "Operario de aseo",
                    company: "Tu Casa Limpia",
                    location: "Medellín",
                    vacancies: 5,
                    qualifications: {
                        a: "No se requiere educación superior",
                        b: "Experiencia en alturas",
                    },
                    salary: "$ 1.2M COP + prestaciones y bonos",
                    posting_date: "22/04/2023"
                },
                {
                    name: "Auxiliar de cocina",
                    company: "La Rioja",
                    location: "Cartagena",
                    vacancies: 1,
                    qualifications: {
                        a: "Curso de manipulación de alimentos",
                        b: "Buena presentación",
                        c: "Profesional en culinaria"
                    },
                    salary: "$ 2M COP",
                    posting_date: "30/04/2023"
                },
                {
                    name: "DevOps",
                    company: "Array World",
                    location: "Remoto",
                    vacancies: 1,
                    qualifications: {
                        a: "Azure Cloud",
                        b: "Python",
                        c: "Node JS"
                    },
                    salary: "$ 7M COP",
                    posting_date: "19/04/2023"
                },
                {
                    name: "Call Center (Medio tiempo)",
                    company: "BCall",
                    location: "Bogotá",
                    vacancies: 15,
                    qualifications: {
                        a: "Servicio al cliente",
                        b: "Inglés C1",
                        c: "Herramientas ofimáticas"
                    },
                    salary: "$ 2M COP + prestaciones y bonos",
                    posting_date: "28/04/2023"
                },
            ],

        }
    },
}

</script>

<style scoped>
.jobPosting {
    border: 1px solid gray;
    border-radius: 5px;
}

.jobPosting:hover {
    box-shadow: 4px 2px 4px 1px rgb(126, 124, 124);
    cursor: pointer;
    transition: all .2s ease;
}

.jobLink {
    text-decoration: none;
}

.my-logo {
    width: 100%;
}

.habilidad {
    font-size: 14px;
    border-radius: 10px;
    display: inline-block;
    padding: 0 .5rem;
    margin: 0 .25rem;
    cursor: pointer;
    transition: all .2s ease;
}
</style>