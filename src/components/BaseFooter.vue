<template>
    <footer class="base-footer">
        <div class="footer-content">
            <p class="footer-text">
                © 2025 Mon Application - Luka tp3
            </p>
        </div>
    </footer>
</template>

<script>

export default {
  name: 'BaseFooter'
}
</script>

<style scoped>
.base-footer {
  background-color: #2c3e50;
  width: 100%;
  padding: 0;
  position: fixed;
  bottom: 0;
  left: 0;
  z-index: 1000;
}


.footer-content {
  padding: 20px;
  text-align: center;
}

.footer-text {
  color: #ffffff;
  font-size: 14px;
  margin: 0;
}

</style>