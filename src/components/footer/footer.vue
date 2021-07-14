

<script>
import './footer.css';
export default {
  name: 'Footer',
  props: {
    anio:{
          default:new Date().getFullYear()
      }
  }
}
</script>

<template>
  <div class="foter">
    <footer class="footer bg-dark">
        <div class="container">
        <p align="center">
            &copy; Unipamplona {{anio}}
        </p>
        </div>
    </footer>
  </div>
</template>
