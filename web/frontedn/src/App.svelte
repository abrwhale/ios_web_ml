<script>
    let fronend_message;
  
    fetch("http://127.0.0.1:8000/").then((response) => {
      response.json().then((json) => {
        fronend_message = json.backend_message;
      });
    });
  </script>
  
  <h1>{fronend_message}</h1>