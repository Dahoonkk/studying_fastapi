<script>
  let message;

  fetch("http://localhost:8000/api/question/list").then((response) => {
    response.json().then((json) => {
      message = json.message;
    })
  })
</script>

<h1>{message}</h1>