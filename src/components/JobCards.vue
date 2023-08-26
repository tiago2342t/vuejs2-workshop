<template>
    <div class="card">
      <div class="card-body" v-for="(empleo, indice) in empleos" :key="indice">
        <h5 class="card-title">{{ empleo.name }}</h5>
        <h6 class="card-subtitle mb-2 text-muted">{{ empleo.company }}</h6>
        <p class="card-text">{{ empleo.location }}</p>
        <ul>
            <li v-for="(qual, index) in empleo.qualifications" :key="index">{{ qual }}</li>
        </ul>
        <a href="#" class="card-link">{{ empleo.salary }}</a>
        <a href="#" class="card-link">{{ empleo.posting_date }}</a>
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
</style>