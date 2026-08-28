برای GitHub Pages:

1. manifest.webmanifest را کنار index.html در ریشه Repository آپلود کن.
2. service-worker.js را هم کنار index.html آپلود کن.
3. پوشه icons را در ریشه Repository قرار بده.
4. در index.html داخل <head> این خط باید وجود داشته باشد:
<link rel="manifest" href="./manifest.webmanifest">
5. برای Service Worker، قبل از </body> این کد باید وجود داشته باشد:
<script>
if ("serviceWorker" in navigator) {
  window.addEventListener("load", () => {
    navigator.serviceWorker.register("./service-worker.js", {scope: "./"});
  });
}
</script>
