<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Redirecting...</title>
  <script>
    (function () {
      const urlParams = new URLSearchParams(window.location.search);
      const target = urlParams.get("redirect_to");
      if (target) {
        // Перебрасываем из WebApp наружу
        window.top.location.href = target;
      } else {
        document.body.innerText = "No redirect target";
      }
    })();
  </script>
</head>
<body>
  Перенаправление...
</body>
</html>
