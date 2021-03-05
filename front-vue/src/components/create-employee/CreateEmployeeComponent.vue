<template>
  <div class="container">
    <div class="card">
      <div class="card-header">
        <h3>Add Employee</h3>
      </div>
      <div class="card-body">
        <form v-on:submit.prevent="handleSubmitForm()">
          <!-- INÍCIO BLOCO: Employee Name -->
          <div class="form-group">
            <label class="font-weight-bold">Employee name</label>
            <input
              type="text"
              placeholder="Type Your name"
              class="form-control"
              v-model="employee.name"
              required
            />
          </div>
          <!-- FIM BLOCO: Employee Name -->

          <!-- INÍCIO BLOCO: Jobe Role -->
          <div class="form-group">
            <label class="font-weight-bold">Job Role</label>
            <input
              type="text"
              placeholder="Type Your Job Role"
              class="form-control"
              v-model="employee.job_rule"
              required
            />
          </div>
          <!-- FIM BLOCO: Jobe Role -->

          <!-- INÍCIO BLOCO: Salary -->
          <div class="form-group">
            <label class="font-weight-bold">Salary</label>
            <input
              type="number"
              placeholder="Type Your Salary"
              class="form-control"
              v-model="employee.salary"
              required
            />
          </div>
          <!-- FIM BLOCO: salary -->

          <!-- INÍCIO BLOCO: Birth -->
          <div class="form-group">
            <label class="font-weight-bold">Birth</label>
            <input
              type="date"
              placeholder="YYYY/MM/DD"
              v-model="employee.birth"
              required
              class="form-control"
            />
          </div>
          <!-- FIM BLOCO: Birth -->

          <!-- INÍCIO BLOCO: Employee Registration -->
          <div class="form-group">
            <label class="font-weight-bold">Employee Registration</label>
            <input
              type="text"
              placeholder="Employee Registration"
              class="form-control"
              v-model="employee.employee_registration"
              required
            />
          </div>
          <!-- FIM BLOCO: Employee Registration -->
          <div class="form-group">
            <button class="btn btn-primary" type="submit">+ Employee</button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {
    name: 'CreateEmployeeComponent',
  },
  data() {
    return {
      employee: {
        name: '',
        job_role: '',
        salary: '',
        birth: '',
        employee_registration: '',
      },
    };
  },
  methods: {
    handleSubmitForm() {

    },
  },
};
</script>
